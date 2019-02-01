# API POST to Class vzBrCP

This POST will create a new {{contract-name}} in {{tn-name}} without a subject. The scope of the contract is defined as "scope".

POST to `https://{{apic}}/api/node/mo/.json?rsp-subtree=modified`

``` json
{
  "vzBrCP": {
    "attributes": {
      "annotation": "",
      "descr": "",
      "dn": "uni/tn-{{tn-name}}/brc-{{contract-name}}",
      "name": "{{contract-name}}",
      "nameAlias": "",
      "ownerKey": "",
      "ownerTag": "",
      "prio": "unspecified",
      "scope": "context",
      "targetDscp": "unspecified",
      "status": "created,modified"
    }
  }
}
```
