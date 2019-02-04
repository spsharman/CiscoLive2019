# API query to Class fvRsProv and fvRsCons

This call will query the fvRsProv and fvRsCons Classes to retrieve details from the {{tn-name}}/{{ap-name}}/{{epg-name}}.

`https://{{apic}}/api/node/mo/uni/tn-{{tn-name}}/ap-{{ap-name}}/epg-{{epg-name}}.json?query-target=subtree&target-subtree-class=fvRsProv&target-subtree-class=fvRsCons`


## Example output

```json
{
    "totalCount": "8",
    "imdata": [
        {
            "fvRsProv": {
                "attributes": {
                    "annotation": "",
                    "childAction": "",
                    "ctrctUpd": "ctrct",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/rsprov-default",
                    "extMngdBy": "",
                    "forceResolve": "yes",
                    "lcOwn": "local",
                    "matchT": "AtleastOne",
                    "modTs": "2019-01-30T11:14:05.558+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "prio": "unspecified",
                    "rType": "mo",
                    "state": "formed",
                    "stateQual": "none",
                    "status": "",
                    "tCl": "vzBrCP",
                    "tContextDn": "",
                    "tDn": "uni/tn-common/brc-default",
                    "tRn": "brc-default",
                    "tType": "name",
                    "tnVzBrCPName": "default",
                    "triggerSt": "triggerable",
                    "uid": "15374",
                    "updateCollection": "no"
                }
            }
        },
        {
            "fvRsProv": {
                "attributes": {
                    "annotation": "",
                    "childAction": "",
                    "ctrctUpd": "ctrct",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/rsprov-permit_any-any",
                    "extMngdBy": "",
                    "forceResolve": "yes",
                    "lcOwn": "local",
                    "matchT": "AtleastOne",
                    "modTs": "2019-01-30T11:14:05.558+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "prio": "unspecified",
                    "rType": "mo",
                    "state": "formed",
                    "stateQual": "none",
                    "status": "",
                    "tCl": "vzBrCP",
                    "tContextDn": "",
                    "tDn": "uni/tn-rwhitear/brc-permit_any-any",
                    "tRn": "brc-permit_any-any",
                    "tType": "name",
                    "tnVzBrCPName": "permit_any-any",
                    "triggerSt": "triggerable",
                    "uid": "15194",
                    "updateCollection": "no"
                }
            }
        },
        {
            "fvRsProv": {
                "attributes": {
                    "annotation": "",
                    "childAction": "",
                    "ctrctUpd": "ctrct",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/rsprov-permit_to_ccc",
                    "extMngdBy": "",
                    "forceResolve": "yes",
                    "lcOwn": "local",
                    "matchT": "AtleastOne",
                    "modTs": "2019-01-30T11:14:05.558+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "prio": "unspecified",
                    "rType": "mo",
                    "state": "formed",
                    "stateQual": "none",
                    "status": "",
                    "tCl": "vzBrCP",
                    "tContextDn": "",
                    "tDn": "uni/tn-rwhitear/brc-permit_to_ccc",
                    "tRn": "brc-permit_to_ccc",
                    "tType": "name",
                    "tnVzBrCPName": "permit_to_ccc",
                    "triggerSt": "triggerable",
                    "uid": "15194",
                    "updateCollection": "no"
                }
            }
        },
        {
            "fvRsProv": {
                "attributes": {
                    "annotation": "",
                    "childAction": "",
                    "ctrctUpd": "ctrct",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/rsprov-permit_to_CloudCenter_CCC",
                    "extMngdBy": "",
                    "forceResolve": "yes",
                    "lcOwn": "local",
                    "matchT": "AtleastOne",
                    "modTs": "2019-01-30T11:14:05.558+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "prio": "unspecified",
                    "rType": "mo",
                    "state": "formed",
                    "stateQual": "none",
                    "status": "",
                    "tCl": "vzBrCP",
                    "tContextDn": "",
                    "tDn": "uni/tn-rwhitear/brc-permit_to_CloudCenter_CCC",
                    "tRn": "brc-permit_to_CloudCenter_CCC",
                    "tType": "name",
                    "tnVzBrCPName": "permit_to_CloudCenter_CCC",
                    "triggerSt": "triggerable",
                    "uid": "15374",
                    "updateCollection": "no"
                }
            }
        },
        {
            "fvRsCons": {
                "attributes": {
                    "annotation": "",
                    "childAction": "",
                    "ctrctUpd": "ctrct",
                    "deplInfo": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/rscons-permit_to_ipam",
                    "extMngdBy": "",
                    "forceResolve": "yes",
                    "lcOwn": "local",
                    "modTs": "2019-01-30T11:14:05.558+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "prio": "unspecified",
                    "rType": "mo",
                    "state": "formed",
                    "stateQual": "none",
                    "status": "",
                    "tCl": "vzBrCP",
                    "tContextDn": "",
                    "tDn": "uni/tn-common/brc-permit_to_ipam",
                    "tRn": "brc-permit_to_ipam",
                    "tType": "name",
                    "tnVzBrCPName": "permit_to_ipam",
                    "triggerSt": "triggerable",
                    "uid": "15374",
                    "updateCollection": "no"
                }
            }
        },
        {
            "fvRsCons": {
                "attributes": {
                    "annotation": "",
                    "childAction": "",
                    "ctrctUpd": "ctrct",
                    "deplInfo": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/rscons-permit_any-any",
                    "extMngdBy": "",
                    "forceResolve": "yes",
                    "lcOwn": "local",
                    "modTs": "2019-01-30T11:14:05.558+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "prio": "unspecified",
                    "rType": "mo",
                    "state": "formed",
                    "stateQual": "none",
                    "status": "",
                    "tCl": "vzBrCP",
                    "tContextDn": "",
                    "tDn": "uni/tn-rwhitear/brc-permit_any-any",
                    "tRn": "brc-permit_any-any",
                    "tType": "name",
                    "tnVzBrCPName": "permit_any-any",
                    "triggerSt": "triggerable",
                    "uid": "15374",
                    "updateCollection": "no"
                }
            }
        },
        {
            "fvRsCons": {
                "attributes": {
                    "annotation": "",
                    "childAction": "",
                    "ctrctUpd": "ctrct",
                    "deplInfo": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/rscons-permit_to_DSERVER_1",
                    "extMngdBy": "",
                    "forceResolve": "yes",
                    "lcOwn": "local",
                    "modTs": "2019-01-30T11:14:05.558+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "prio": "unspecified",
                    "rType": "mo",
                    "state": "formed",
                    "stateQual": "none",
                    "status": "",
                    "tCl": "vzBrCP",
                    "tContextDn": "",
                    "tDn": "uni/tn-rwhitear/brc-permit_to_DSERVER_1",
                    "tRn": "brc-permit_to_DSERVER_1",
                    "tType": "name",
                    "tnVzBrCPName": "permit_to_DSERVER_1",
                    "triggerSt": "triggerable",
                    "uid": "15374",
                    "updateCollection": "no"
                }
            }
        },
        {
            "fvRsCons": {
                "attributes": {
                    "annotation": "",
                    "childAction": "",
                    "ctrctUpd": "ctrct",
                    "deplInfo": "",
                    "dn": "uni/tn-rwhitear/ap-CloudCenter/epg-CCC/rscons-permit_to_CloudCenter_CCC",
                    "extMngdBy": "",
                    "forceResolve": "yes",
                    "lcOwn": "local",
                    "modTs": "2019-01-30T11:14:05.558+00:00",
                    "monPolDn": "uni/tn-common/monepg-default",
                    "prio": "unspecified",
                    "rType": "mo",
                    "state": "formed",
                    "stateQual": "none",
                    "status": "",
                    "tCl": "vzBrCP",
                    "tContextDn": "",
                    "tDn": "uni/tn-rwhitear/brc-permit_to_CloudCenter_CCC",
                    "tRn": "brc-permit_to_CloudCenter_CCC",
                    "tType": "name",
                    "tnVzBrCPName": "permit_to_CloudCenter_CCC",
                    "triggerSt": "triggerable",
                    "uid": "15374",
                    "updateCollection": "no"
                }
            }
        }
    ]
}
```
