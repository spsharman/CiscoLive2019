# API query to Class fvCEp

This call will query the fvCEp Class to retrieve the {{endpoint-ip-address}} details by range.

Output can be restricted by removing the subtree-class queries.

`https://{{apic}}/api/node/class/fvCEp.json?query-target-filter=and(ge(fvCEp.ip,"{{endpoint-ip-address-start}}")le(fvCEp.ip,"{{endpoint-ip-address-end}}"))&rsp-subtree=children&rsp-subtree-class=fvRsToVm&rsp-subtree-class=fvRsVm&rsp-subtree-class=fvRsHyper&rsp-subtree-class=fvRsCEpToPathEp&rsp-subtree-class=fvIp&rsp-subtree-class=fvPrimaryEncap&order-by=fvCEp.ip`


## Example output

```json
{
  "totalCount": "2",
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
    },
    {
      "fvCEp": {
        "attributes": {
          "annotation": "",
          "childAction": "",
          "contName": "",
          "dn": "uni/tn-rwhitear/ap-Ubuntu/epg-Ubuntu/cep-00:50:56:A2:C5:28",
          "encap": "vlan-2097",
          "extMngdBy": "",
          "id": "0",
          "idepdn": "",
          "ip": "10.52.249.121",
          "lcC": "vmm",
          "lcOwn": "local",
          "mac": "00:50:56:A2:C5:28",
          "mcastAddr": "not-applicable",
          "modTs": "2018-08-07T18:34:02.498+00:00",
          "monPolDn": "uni/tn-common/monepg-default",
          "name": "00:50:56:A2:C5:28",
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
                "modTs": "2018-06-20T09:23:19.195+00:00",
                "rType": "mo",
                "rn": "rsvm",
                "state": "formed",
                "stateQual": "none",
                "status": "",
                "tCl": "compVm",
                "tDn": "comp/prov-VMware/ctrlr-[rwhitear-vds-01]-rwhitear-vc01/vm-vm-314",
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
                "modTs": "2018-06-20T09:23:19.195+00:00",
                "rType": "mo",
                "rn": "rstoVm-[comp/prov-VMware/ctrlr-[rwhitear-vds-01]-rwhitear-vc01/vm-vm-314]",
                "state": "formed",
                "stateQual": "none",
                "status": "",
                "tCl": "compVm",
                "tDn": "comp/prov-VMware/ctrlr-[rwhitear-vds-01]-rwhitear-vc01/vm-vm-314",
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
                "modTs": "2018-09-24T08:42:51.675+00:00",
                "rType": "mo",
                "rn": "rshyper-[comp/prov-VMware/ctrlr-[rwhitear-vds-01]-rwhitear-vc01/hv-host-483]",
                "state": "formed",
                "stateQual": "none",
                "status": "",
                "tCl": "compHv",
                "tDn": "comp/prov-VMware/ctrlr-[rwhitear-vds-01]-rwhitear-vc01/hv-host-483",
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
                "modTs": "2018-09-24T08:42:51.709+00:00",
                "rType": "mo",
                "rn": "rscEpToPathEp-[topology/pod-1/paths-101/pathep-[eth1/83]]",
                "state": "formed",
                "stateQual": "none",
                "status": "",
                "tCl": "fabricAPathEp",
                "tDn": "topology/pod-1/paths-101/pathep-[eth1/83]",
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
                "modTs": "2018-09-24T08:42:51.675+00:00",
                "rType": "mo",
                "rn": "rscEpToPathEp-[topology/pod-1/paths-102/pathep-[eth1/83]]",
                "state": "formed",
                "stateQual": "none",
                "status": "",
                "tCl": "fabricAPathEp",
                "tDn": "topology/pod-1/paths-102/pathep-[eth1/83]",
                "tType": "mo"
              }
            }
          }
        ]
      }
    }
  ]
}
```
