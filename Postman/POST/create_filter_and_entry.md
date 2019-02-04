# API POST to distinguished name {{tn-name}}/{{filter-name}}

This POST will create a new {{filter-name}} with a filter entry containing the source and destination ports.

POST to `https://{{apic}}/api/node/mo/uni/tn-{{tn-name}}/flt-{{filter-name}}.json?rsp-subtree=modified`

``` json
{
  "vzFilter": {
    "attributes": {
      "annotation": "",
      "descr": "",
      "dn": "uni/tn-{{tn-name}}/flt-{{filter-name}}",
      "name": "{{filter-name}}",
      "nameAlias": "",
      "ownerKey": "",
      "ownerTag": "",
      "status": "created,modified"
    },
    "children": [
      {
        "vzEntry": {
          "attributes": {
            "annotation": "",
            "applyToFrag": "no",
            "arpOpc": "unspecified",
            "dFromPort": "{{dst-from-port}}",
            "dToPort": "{{dst-to-port}}",
            "descr": "",
            "etherT": "ip",
            "icmpv4T": "unspecified",
            "icmpv6T": "unspecified",
            "matchDscp": "unspecified",
            "name": "{{filter-name}}",
            "nameAlias": "",
            "prot": "tcp",
            "sFromPort": "{{src-from-port}}",
            "sToPort": "{{src-to-port}}",
            "stateful": "no",
            "tcpRules": "",
            "status": "created,modified"
          }
        }
      }
    ]
  }
}
```
