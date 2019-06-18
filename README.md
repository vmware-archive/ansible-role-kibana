# ansible-role-kibana

Ansible playbook to automate installing and maintaining kibana as containers.

## Requirements

This role currently requires a working VMware Photon server with enabled Docker environment.

## Role Variables

```yaml
# Container memory limit. Use 512MB, type string, or 0 for unlimited
memory_limit: 0MB

# Directy into which to place temporary files during the image build.
kibana_docker_build: /tmp/kibana

# The container image name to build and use.
kibana_docker_image: vmware-opencloud/kibana

# The elasticsearch cluster to bind.
elasticsearch_cluster_name: default_clustername
```

## Example playbook

```yaml
---
- hosts: kibana
  sudo: True
  roles:
    - kibana
  vars:
    - ... forthcoming
```

# License and Copyright
 
Copyright 2015 VMware, Inc.  All rights reserved.

SPDX-License-Identifier: Apache-2.0 OR GPL-3.0-only

This code is Dual Licensed Apache-2.0 or GPLv3

