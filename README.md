# Docker

## Install

```
tasks:
- name: "Install docker"
  import_role:
    name: docker
    tasks_from: install.yml
```

or using tags `ansible-playbook docker.yml -i inventory.yml --tags install`

```
tasks:
- name: "Install docker"
  roles:
    - docker
```


## Configure

Configure ring log.

```
- name: "Configure docker"
  import_role:
    name: docker
    tasks_from: configure.yml
```


## Install python modules

```
- name: "Configure python modules for docker"
  import_role:
    name: docker
    tasks_from: python.yml
```
