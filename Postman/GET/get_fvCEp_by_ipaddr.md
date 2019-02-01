# API call

This call will query the fvCEp Class to retrieve {{endpoint-ip-address}} details.

`https://{{apic}}/api/node/class/fvCEp.json?query-target-filter=and(eq(fvCEp.ip,"{{endpoint-ip-address}}"))&rsp-subtree=children&rsp-subtree-class=fvRsToVm&rsp-subtree-class=fvRsVm&rsp-subtree-class=fvRsHyper&rsp-subtree-class=fvRsCEpToPathEp&rsp-subtree-class=fvIp&rsp-subtree-class=fvPrimaryEncap&order-by=fvCEp.ip`


## Example output

```json
{
    "totalCount": "1",
    "imdata": [
        {
            "fvCEp": {
                "attributes": {
                    "annotation": "",
                    "childAction": "",
                    "contName": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/cep-00:50:56:A2:6A:A9",
                    "encap": "vlan-2086",
                    "extMngdBy": "",
                    "id": "0",
                    "idepdn": "",
                    "ip": "10.52.249.120",
                    "lcC": "learned,vmm",
                    "lcOwn": "local",
                    "mac": "00:50:56:A2:6A:A9",
                    "mcastAddr": "not-applicable",
                    "modTs": "2018-11-13T23:59:11.829+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "name": "00:50:56:A2:6A:A9",
                    "nameAlias": "",
                    "status": "",
                    "uid": "0",
                    "uuid": "",
                    "vmmSrc": "dvs"
                },
                "children": [
                    {
                        "fvRsVm": {
                            "attributes": {
                                "childAction": "",
                                "forceResolve": "yes",
                                "lcOwn": "local",
                                "modTs": "2018-10-11T07:41:39.589+00:00",
                                "rType": "mo",
                                "rn": "rsvm",
                                "state": "formed",
                                "stateQual": "none",
                                "status": "",
                                "tCl": "compVm",
                                "tDn": "comp/prov-VMware/ctrlr-[rwhitear-vds-01]-rwhitear-vc01/vm-vm-1298",
                                "tType": "mo"
                            }
                        }
                    },
                    {
                        "fvRsToVm": {
                            "attributes": {
                                "childAction": "",
                                "forceResolve": "yes",
                                "isBootstrapUpd": "attach",
                                "lcOwn": "local",
                                "modTs": "2018-10-11T07:41:39.589+00:00",
                                "rType": "mo",
                                "rn": "rstoVm-[comp/prov-VMware/ctrlr-[rwhitear-vds-01]-rwhitear-vc01/vm-vm-1298]",
                                "state": "formed",
                                "stateQual": "none",
                                "status": "",
                                "tCl": "compVm",
                                "tDn": "comp/prov-VMware/ctrlr-[rwhitear-vds-01]-rwhitear-vc01/vm-vm-1298",
                                "tType": "mo"
                            }
                        }
                    },
                    {
                        "fvRsHyper": {
                            "attributes": {
                                "childAction": "",
                                "forceResolve": "yes",
                                "isBootstrapUpd": "attach",
                                "lcOwn": "local",
                                "modTs": "2018-10-11T07:44:31.612+00:00",
                                "rType": "mo",
                                "rn": "rshyper-[comp/prov-VMware/ctrlr-[rwhitear-vds-01]-rwhitear-vc01/hv-host-481]",
                                "state": "formed",
                                "stateQual": "none",
                                "status": "",
                                "tCl": "compHv",
                                "tDn": "comp/prov-VMware/ctrlr-[rwhitear-vds-01]-rwhitear-vc01/hv-host-481",
                                "tType": "mo"
                            }
                        }
                    },
                    {
                        "fvRsCEpToPathEp": {
                            "attributes": {
                                "childAction": "",
                                "forceResolve": "yes",
                                "lcC": "learned,vmm",
                                "lcOwn": "local",
                                "modTs": "2018-11-13T23:59:11.829+00:00",
                                "rType": "mo",
                                "rn": "rscEpToPathEp-[topology/pod-1/paths-102/pathep-[eth1/81]]",
                                "state": "formed",
                                "stateQual": "none",
                                "status": "",
                                "tCl": "fabricAPathEp",
                                "tDn": "topology/pod-1/paths-102/pathep-[eth1/81]",
                                "tType": "mo"
                            }
                        }
                    },
                    {
                        "fvRsCEpToPathEp": {
                            "attributes": {
                                "childAction": "",
                                "forceResolve": "yes",
                                "lcC": "vmm",
                                "lcOwn": "local",
                                "modTs": "2018-11-13T23:53:45.540+00:00",
                                "rType": "mo",
                                "rn": "rscEpToPathEp-[topology/pod-1/paths-101/pathep-[eth1/81]]",
                                "state": "formed",
                                "stateQual": "none",
                                "status": "",
                                "tCl": "fabricAPathEp",
                                "tDn": "topology/pod-1/paths-101/pathep-[eth1/81]",
                                "tType": "mo"
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
                                "extMngdBy": "",
                                "lcOwn": "local",
                                "modTs": "2018-12-05T15:28:14.966+00:00",
                                "monPolDn": "uni/tn-common/monepg-default",
                                "rn": "ip-[10.52.249.120]",
                                "status": "",
                                "uid": "0"
                            }
                        }
                    }
                ]
            }
        }
    ]
}
```
