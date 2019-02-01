This playbook will prompt the user to input a Tenant, it will then print all the Bridge Domains for the given Tenant.

Toggle **debug:** true/false to display debug information.

```yaml
---
#Play 1
- name:                 Setup playbook
  hosts:                localhost
  connection:           local
  gather_facts:         no

  vars_prompt:
    - name:             "tenant"
      prompt:           "Get Bridge Domains for a given Tenant (press enter for all Tenants)"
      private:          no

  tasks:
    - name:
      set_fact:
        tenant:         "{{ tn-name }}"
        debug:          false


# Play 2
- name:                 Get all Bridge Domains for a given Tenant
  hosts:                localhost
  connection:           local
  gather_facts:         no

  tasks:
    - name:             Get all Bridge Domains for a given Tenant
      aci_rest:
        host:           "{{ apic }}"
        username:       "{{ apic_username }}"
        password:       "{{ apic_password }}"
        validate_certs: no
        use_proxy:      no
        method:         get
        path:           /api/node/class/fvBD.json?query-target-filter=and(wcard(fvBD.dn,"{{ tn-name }}"))
      register:         all_bridge_domains

    - name:             Create list of Bridge Domains
      set_fact:
        all_bridge_domain_names : "{{ all_bridge_domains | json_query('imdata[*].fvBD.attributes.dn') | sort }}"

    - debug:
        msg:            "{{ all_bridge_domain_names }}"


# Debug
- name:                 Print debug information
  hosts:                localhost
  connection:           local
  gather_facts:         no

  tasks:
    - debug:
        var:            all_bridge_domains
      when:             debug == true

    - debug:
        msg:            all_bridge_domain_names
      when:             debug == true
```
