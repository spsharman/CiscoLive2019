# API query to a specific distinguished name

This call will query the dn {{tn-name}}/{{filter-name}} to retrive the Filter entries.

`https://{{apic}}/api/node/mo/uni/tn-{{tn-name}}/flt-{{filter-name}}.json?query-target=subtree&target-subtree-class=vzEntry`


## Example output

```json
{
    "totalCount": "1",
    "imdata": [
        {
            "vzEntry": {
                "attributes": {
                    "annotation": "",
                    "applyToFrag": "no",
                    "arpOpc": "unspecified",
                    "childAction": "",
                    "dFromPort": "unspecified",
                    "dToPort": "unspecified",
                    "descr": "",
                    "dn": "uni/tn-rwhitear/flt-any/e-any",
                    "etherT": "unspecified",
                    "extMngdBy": "",
                    "icmpv4T": "unspecified",
                    "icmpv6T": "unspecified",
                    "lcOwn": "local",
                    "matchDscp": "unspecified",
                    "modTs": "2018-04-26T11:54:21.509+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "name": "any",
                    "nameAlias": "",
                    "prot": "unspecified",
                    "sFromPort": "unspecified",
                    "sToPort": "unspecified",
                    "stateful": "no",
                    "status": "",
                    "tcpRules": "",
                    "uid": "15374"
                }
            }
        }
    ]
}
```
