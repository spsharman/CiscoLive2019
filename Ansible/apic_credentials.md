This variables file is used to pull in the APIC credentials into a playbook.

`ansible-playbook playbook.yml -e @apic_credentials.yml`

```yaml
---
  apic: apic_fqdn
  apic_ip: apic_ip_address
  apic_username: "username"
  apic_password: "password"
```
