# ansible-role-elasticsearch

Ansible playbook to automate installing and maintaining kibana as containers.

## Requirements

This role currently requires a working VMware Photon server with enabled Docker environment.

## Role Variables

... forthcoming

## Example playbook

```
---
- hosts: kibana
  sudo: True
  roles:
    - kibana
  vars:
    - ... forthcoming
```

# License and Copyright
 
Copyright 2015 VMware, Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

