# federicoantoniazzi.nomad

Install and configure Hashicorp Nomad

## Role Variables
All variables have been taken from the [official documentation page](https://developer.hashicorp.com/nomad/docs/configuration). There you can find a complete reference for the variables scope and usage.

### Generic configuration
[`nomad.yml`](https://github.com/FedericoAntoniazzi/ansible-role-nomad/blob/master/defaults/main/nomad.yml)
### Node configuration
[`nodeconfig.yml`](https://github.com/FedericoAntoniazzi/ansible-role-nomad/blob/master/defaults/main/nodeconfig.yml)
### Client configuration
[`clientconfig.yml`](https://github.com/FedericoAntoniazzi/ansible-role-nomad/blob/master/defaults/main/clientconfig.yml)
### Server configuration
[`serverconfig.yml`](https://github.com/FedericoAntoniazzi/ansible-role-nomad/blob/master/defaults/main/serverconfig.yml)
### Plugin configuration
- [`docker.yml`](https://github.com/FedericoAntoniazzi/ansible-role-nomad/blob/master/defaults/main/docker.yml)
- [`podman.yml`](https://github.com/FedericoAntoniazzi/ansible-role-nomad/blob/master/defaults/main/podman.yml)

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
- name: Install Nomad
  hosts: nomad
  vars:
    nomad_roles: ['server', 'client']
  roles:
    - nomad
```

## License

MIT

## Author Information

FedericoAntoniazzi ([website](https://federicoantoniazzi.dev))
