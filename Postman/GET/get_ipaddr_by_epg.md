# API query to Class fvIp

This call will query the fvIp Class to retrieve the {{endpoint-ip-address}} details from {ap-name}/{epg-name}.

`https://{{apic}}/api/node/class/fvIp.json?query-target-filter=and(wcard(fvIp.dn,"ap-{ap-name}/epg-{epg-name}"))&order-by=fvIp.addr`


## Example output

```json
{
    "totalCount": "18",
    "imdata": [
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.98",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:64:3E/ip-[10.52.249.98]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2019-01-21T14:35:00.136+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.99",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:0B:C5/ip-[10.52.249.99]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2019-01-21T14:30:09.605+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.100",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:7A:0E/ip-[10.52.249.100]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2019-01-21T14:37:40.218+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.101",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:8B:AC/ip-[10.52.249.101]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2019-01-21T14:35:09.661+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.102",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:50:33/ip-[10.52.249.102]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2018-07-19T14:19:19.144+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.103",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:9A:A7/ip-[10.52.249.103]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2019-01-21T14:35:40.169+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.104",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:73:E6/ip-[10.52.249.104]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2019-01-21T14:30:00.107+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.105",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:BA:94/ip-[10.52.249.105]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2019-01-21T14:25:09.550+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.106",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:00:62/ip-[10.52.249.106]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2019-01-21T14:35:49.699+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.107",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:35:AC/ip-[10.52.249.107]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2018-09-11T07:51:29.805+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.108",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:1A:C2/ip-[10.52.249.108]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2019-01-21T14:30:20.099+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.109",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:A1:AC/ip-[10.52.249.109]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2018-11-01T08:57:45.837+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.111",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:6A:F5/ip-[10.52.249.111]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2018-10-25T12:31:25.172+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.117",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:95:AE/ip-[10.52.249.117]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2018-11-02T15:17:10.260+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.118",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:BA:71/ip-[10.52.249.118]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2018-09-11T17:05:57.418+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
        {
            "fvIp": {
                "attributes": {
                    "addr": "10.52.249.119",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:CF:CC/ip-[10.52.249.119]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2018-09-11T11:15:27.917+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        },
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
                    "addr": "10.52.249.124",
                    "annotation": "",
                    "childAction": "",
                    "debugMACMessage": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:9A:DF/ip-[10.52.249.124]",
                    "extMngdBy": "",
                    "lcOwn": "local",
                    "modTs": "2019-01-21T14:24:29.580+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "status": "",
                    "uid": "0"
                }
            }
        }
    ]
}
```
