# API query to a specific distinguished name

This call will query the dn {{tn-name}}/{{contract-name}}.

`https://{{apic}}/api/node/mo/uni/tn-{{tn-name}}/brc-{{contract-name}}.json?query-target=self`


## Example output

```json
{
    "totalCount": "1",
    "imdata": [
        {
            "vzBrCP": {
                "attributes": {
                    "annotation": "",
                    "childAction": "",
                    "configIssues": "",
                    "descr": "",
                    "dn": "uni/tn-rwhitear/brc-permit_to_ccc",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2018-06-20T07:23:32.980+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "name": "permit_to_ccc",
                    "nameAlias": "",
                    "ownerKey": "",
                    "ownerTag": "",
                    "prio": "unspecified",
                    "reevaluateAll": "no",
                    "scope": "context",
                    "status": "",
                    "targetDscp": "unspecified",
                    "uid": "15194"
                }
            }
        }
    ]
}
```
