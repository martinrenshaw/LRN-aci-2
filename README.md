# LRN-aci-2
ACI with var options

```
$ ansible-playbook 05_aci_deploy_app.yml -i inventory --list-tasks

playbook: 05_aci_deploy_app.yml

  play #1 (apic): ENSURE APPLICATION CONFIGURATION EXISTS    TAGS: []
    tasks:
      TASK 01 - ENSURE APPLICATIONS TENANT EXISTS    TAGS: [app, bd, contract, epg, filter, tenant, vrf]
      TASK 02 - ENSURE TENANT VRF EXISTS    TAGS: [bd, vrf]
      TASK 03 - ENSURE TENANT BRIDGE DOMAINS AND EXIST    TAGS: [bd]
      TASK 04 - ENSURE BRIDGE DOMAINS HAVE SUBNETS    TAGS: []
      TASK 05 - ENSURE TENANT FILTERS EXIST    TAGS: [contract, filter]
      TASK 06 - ENSURE FILTERS HAVE FILTER ENTRIES    TAGS: [contract, filter]
      TASK 07 - ENSURE TENANT CONTRACTS EXIST    TAGS: [contract]
      TASK 08 - ENSURE CONTRACTS HAVE CONTRACT SUBJECTS    TAGS: [contract]
      TASK 09 - ENSURE CONTRACT SUBJECTS HAVE FILTERS    TAGS: [contract]
      TASK 10 - ENSURE APPLICATION EXISTS    TAGS: [app, epg]
      TASK 11 - ENSURE APPLICATION EPGS EXISTS    TAGS: [epg]
      TASK 12 - ENSURE DOMAIN IS BOUND TO EPG    TAGS: [epg]
      TASK 13 - ENSURE EPGS HAVE CONTRACTS    TAGS: [epg]
```
