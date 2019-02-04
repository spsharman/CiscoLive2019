# API query to Class fvIp

This call will query the fvIp Class to retrieve the {{endpoint-ip-address}} details from a range.

`https://{{apic}}/api/node/class/fvIp.json?query-target-filter=and(ge(fvIp.addr,"{{endpoint-ip-address-start}}"),le(fvIp.addr,"{{endpoint-ip-address-end}}"))&order-by=fvIp.addr`


## Example output

```json
{
    "totalCount": "3",
    "imdata": [
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.120",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:6A:A9/ip-[10.52.249.120]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2018-12-05T15:28:14.966+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.122",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CSP2100/epg-CSP_Testing/cep-00:FC:BA:73:EB:3C/ip-[10.52.249.122]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2018-06-30T09:41:22.399+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.123",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-Ciscolive/ap-wpCL19_631/epg-WSERVER_1/cep-00:50:56:A2:D8:74/ip-[10.52.249.123]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2019-01-23T14:12:48.153+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        }
    ]
}
```
