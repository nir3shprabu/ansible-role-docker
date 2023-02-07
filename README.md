# Ansible role for Docker

This is a role that will install the Docker CE engine and docker-compose from the official APT repo and perform the [post-installation](https://docs.docker.com/engine/install/linux-postinstall) steps on a Ubuntu target

## Usage

Add this to `requirements.yml`:

```yml
- src: https://github.com/nir3shprabu/ansible-role-docker
  name: 
  version: v<latest-release>
```

### Sample playbook

```yaml
 
- name: "install docker"
  hosts: enter your hosts file
  become: yes
  role:
    - ansible-role-docker

```