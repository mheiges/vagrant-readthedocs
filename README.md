
# A Read the Docs Demo

Installs a Read The Docs server on a Vagrant/VirtualBox virtual machine.

Accessible on host at http://rtfd.vm/


## Requirements

- Install VirtualBox
- Install Vagrant
  - install landrush plugin
- Install Ansible
- git checkout vagrant-readthedocs

## Setup

    cd vagrant-readthedocs
    vagrant up

_The installation sometimes fails with pip errors (usually network related). Run `vagrant provision` to try again._

Point browser at
    http://rtfd.vm/


## Admin

Superuser name and password is set at the top of the `playbook.yml` file.