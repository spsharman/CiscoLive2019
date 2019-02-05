This playbook will prompt the user to input a Tenant, it will then print all Application Profiles and EPGs for the given Tenant.

Toggle **debug:** true/false to display debug information.


```yaml
---
#Play 1
- name:                        Setup playbook
  hosts:                       localhost
  connection:                  local
  gather_facts:                no

  vars_prompt:
    - name:                    "tn-name"
      prompt:                  "Enter Tenant name (press enter for all Tenants)"
      private:                 no

  tasks:
    - name:
      set_fact:
        tn-name:                "{{ tn-name }}"
        debug:                 false


# Play 2
- name:                        Get ACI Tenants
  hosts:                       localhost
  connection:                  local
  gather_facts:                no

  tasks:
    - name:                    Get all Tenants
      aci_rest:
        host:                  "{{ apic }}"
        username:              "{{ apic_username }}"
        password:              "{{ apic_password }}"
        validate_certs:        no
        use_proxy:             no
        method:                get
        path:                  /api/node/class/fvTenant.json?query-target-filter=and(wcard(fvTenant.name,"{{ tn-name }}"))
      register:                all_tenants

    - name:                    Create list of Tenant names
      set_fact:
        all_tenant_names:      "{{ all_tenants | json_query('imdata[*].fvTenant.attributes.dn') | sort }}"

    - debug:
        msg:                   "{{ all_tenant_names }}"


# Play 3
- name:                        Get Application Profiles
  hosts:                       localhost
  connection:                  local
  gather_facts:                no

  tasks:
    - name:                    Get all Application Profiles
      aci_rest:
        host:                  "{{ apic }}"
        username:              "{{ apic_username }}"
        password:              "{{ apic_password }}"
        validate_certs:        no
        use_proxy:             no
        method:                get
        path:                  /api/node/class/fvAp.json?query-target-filter=and(wcard(fvAp.dn,"{{ tn-name }}"))
      register:                all_app_profiles

    - name:                    Create list of Application Profile names
      set_fact:
        all_app_profile_names: "{{ all_app_profiles | json_query('imdata[*].fvAp.attributes.dn') | sort }}"

    - debug:
        msg:                   "{{ all_app_profile_names }}"


# Play 4
- name:                        Get EPGs
  hosts:                       localhost
  connection:                  local
  gather_facts:                no

  tasks:
    - name:                    Get all EPGs
      aci_rest:
        host:                  "{{ apic }}"
        username:              "{{ apic_username }}"
        password:              "{{ apic_password }}"
        validate_certs:        no
        use_proxy:             no
        method:                get
        path:                  /api/node/class/fvAEPg.json?query-target-filter=and(wcard(fvAEPg.dn,"{{ tn-name }}"))
      register:                all_epgs

    - name:                    Create list of EPG names
      set_fact:
        all_epg_names:         "{{ all_epgs | json_query('imdata[*].fvAEPg.attributes.dn') | sort }}"

    - debug:
        msg:                   "{{ all_epg_names }}"


# Debug
- name:                        Print debug information
  hosts:                       localhost
  connection:                  local
  gather_facts:                no

  tasks:
    - debug:
        var:                   all_tenants
      when:                    debug == true

    - debug:
        msg:                   all_tenant_names
      when:                    debug == true

    - debug:
        var:                   all_app_profiles
      when:                    debug == true

    - debug:
        msg:                   all_app_profile_names
      when:                    debug == true

    - debug:
        var:                   all_epgs
      when:                    debug == true

    - debug:
        msg:                   all_epg_names
      when:                    debug == true
```
