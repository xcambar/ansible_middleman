# Middleman Ansible

A (pretty successful) experiment to learn [Ansible](http://ansible.co)
with a simple example: A static website with [Middleman](http://middlemanapp.com).

## Requirements

* Ansible 1.6

## Setup

1. Copy your public SSH key to keys/access.pub
1. Copy the private deploy key to kkeys/deploy
1. Populate the `website` section of the `hosts` file
1. Update `variables/project.yml` as per your project's settings

## Playbooks

### Provision

`ansible-playbooks -i hosts ./provision.yml -u root`

### Deploy

`ansible-playbook -i hosts ./deploy.yml -u root`

## Enhancements

* Better user settings (who runs what when)

## Licence

MIT

## Thanks

* The Ansible team and community
* The authors of the various roles used in the playbooks

## Author

Xavier Cambar
