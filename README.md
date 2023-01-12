## A Cybersecurity Playbook/Workflow Metadata Template for Knowledge Management

This repository presents a standard metadata template to support programmatic knowledge management of security playbooks/orchestration workflows.

The template was first introduced in: *Mavroeidis, V., Eis, P., Zadnik, M., Caselli, M., & Jordan, B. (2021, December). On the Integration of Course of Action Playbooks into Shareable Cyber Threat Intelligence. In 2021 IEEE International Conference on Big Data (Big Data) (pp. 2104-2108). IEEE.*

The authors' version of the publication can be accessed at: https://arxiv.org/pdf/2110.10540.pdf

This template has been referenced, implemented, and possibly will be enhanced by several Cyber Threat Intelligence sharing and management technologies such as STIX, [MISP](https://www.misp-project.org/objects.html#_security_playbook), and the OASIS Threat Actor Context Ontology (to name a few).

Products that utilize this template or enhanced versions won't be reflected in this repository, meaning that this repository will remain unchanged and will stay here for educational purposes. 

| Element | Description |
| :--- | :--- |
| **playbook id** | A value that uniquely identifies the playbook. This will be a different ID than the one a structured playbook can possibly carry within. |
| **description** | An explanation, details, and more context about what the playbook does and tries to accomplish. |
| **playbook creation time** | The time at which the playbook was originally created. |
| **playbook modification time** | The time at which the playbook was last modified. |
| **revoked** | A boolean that identifies if the playbook is no longer valid. |
| **playbook creator** | The entity that created this playbook. It can be, for example, a natural person or an organization. It may be represented using a unique identifier that identifies the creator. |
| **playbook valid from** | The time from which the playbook is considered valid and the steps that it contains can be executed. |
| **playbook valid until** | The time at which this playbook should no longer be considered a valid playbook to be executed. |
| **labels** | A set of labels for the playbook (e.g., adversary persona names, associated groups, or malware family/variant/name that this playbook is related to). |
| **organization type** | The type of organization that the playbook is intended for. This can be an industry sector. |
| **playbook standard** | The standard/format/notation the playbook conforms to (e.g., CACAO, BPMN). |
| **playbook abstraction** | The playbook's level of abstraction (e.g., template, executable).  |
| **playbook type** | The operational roles this playbook addresses (e.g., notification, detection, investigation, prevention, mitigation, remediation, attack). |
| **playbook impact** | From 0 to 100, an integer representing the impact the playbook has on the organization. A value of 0 means specifically undefined. Impact values range from 1, the lowest impact, to a value of 100, the highest. For example, a purely investigative playbook that is non-invasive could have a low impact value of 1. In contrast, a playbook that performs changes such as adding rules into a firewall should have a higher impact value. |
| **playbook severity** | From 0 to 100, an integer representing the seriousness of the conditions that this playbook addresses. A value of 0 means specifically undefined. Severity values range from 1, the lowest severity, to a value of 100, the highest. |
| **playbook priority** | From 0 to 100, an integer representing the priority of this playbook relative to other defined playbooks. A value of 0 means specifically undefined. Priority values range from 1, the highest priority, to a value of 100, the lowest. |
| **playbook** | The property that will carry the playbook itself. Playbook producers and consumers use this property to share and retrieve playbooks. |
