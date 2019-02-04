# API POST to distinguished name {{tn-name}}/{{contract-name}}/{{subj-name}}

This POST will add a Subject and Filter to an existing contract.

POST to `https://{{apic}}/api/node/mo/uni/tn-{{tn-name}}/brc-{{contract-name}}/subj-{{subject-name}}.json?rsp-subtree=modified`

``` json
{
  "vzSubj": {
    "attributes": {
      "annotation": "",
      "consMatchT": "AtleastOne",
      "descr": "",
      "dn": "uni/tn-{{tn-name}}/brc-{{contract-name}}/subj-{{subject-name}}",
      "name": "{{subject-name}}",
      "nameAlias": "",
      "prio": "unspecified",
      "provMatchT": "AtleastOne",
      "revFltPorts": "yes",
      "targetDscp": "unspecified",
      "status": "created,modified"
    },
    "children": [
      {
        "vzRsSubjFiltAtt": {
          "attributes": {
            "action": "permit",
            "annotation": "",
            "directives": "",
            "priorityOverride": "default",
            "tnVzFilterName": "{{filter-name}}",
            "status": "created,modified"
          }
        }
      }
    ]
  }
}
```
