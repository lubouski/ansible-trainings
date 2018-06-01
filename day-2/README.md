## How to

This is refactored ansible project for user creation on ubuntu or centos

## Prerequirements

* [Docker](https://docs.docker.com/install/) - Get Docker for your distro
* [Ansible](http://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) - GetAnsible
* [Git](https://git-scm.com/downloads) - Get Git to clone the repo

## How to run on Docker

```
$ docker run -d centos sleep infinity
$ docker run -d ubuntu sleep infinity
$ docker ps
$ ansible-playbook flat-provision.yml -i 'ubuntu-container-name,' -c docker
$ ansible-playbook flat-provision.yml -i 'centos-container-name,' -c docker
$ ansible-playbook playbook.yml -i 'ubuntu-container-name,' -c docker
$ ansible-playbook playbook.yml -i 'centos-container-name,' -c docker 
```





