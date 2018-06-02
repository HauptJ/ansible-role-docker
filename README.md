# ansible-role-docker
Ansible role to install Docker and optionally configure Docker Swarm

[![Build Status] **Coming soon**

## Requirements
- Ansible 2.3+
- CentOS 7

## Installation
1. Fork this repository
2. git submodule add <git host> roles/ansible-role-mariadb
    - [submodule reference](https://chrisjean.com/git-submodules-adding-using-removing-and-updating/)

**Ansible Galaxy:** [HauptJ.docker] **Coming soon**


## Variables

### Docker

| Name                              | Default                                   | Description                             |
|-----------------------------------|-------------------------------------------|-----------------------------------------|
| docker_user                       | vagrant                                   | user to be added to docker group        |
| docker_compose_ver                | 1.18.0                                    | Docker Compose version to install       |
| docker_swarm_state                | disabled                                  | Docker swarm node state. NOTE: Set to disabled to not use swarm mode.|
| docker_swarm_master_ip            | 127.0.0.1                                 | IP address of Docker Swarm master node / advertise-address|
| docker_swarm_master_port          | 2377                                      | Listening port for the master node      |
| docker_swarm_join_token           | some_string                               | Docker Swarm join token to connect to the master node|
