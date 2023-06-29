# Nix Playbook

## Requirements

Ansible installed: on Debian or Molecule you can just run:

   ```sh
   sudo apt install python3-pip
   pip3 install --user ansible
   ```

## Installation

Download and extract this playbook or clone this repository to your local drive.

   ```sh
   git clone git@github.com:staticdev/nix-playbook.git
   ```

## Reproduce with molecule

  ```sh
  pip3 install 'molecule' 'molecule-plugins[podman]'
  molecule -v test > output.txt
  ```

## Reproduce on Debian

Run the command on Debian:

   ```sh
   ansible-galaxy install -fr requirements.yml
   ansible-playbook main.yml -i inventory --ask-become-pass
   ```

## License

Distributed under the terms of the [MIT] license,
_Linux Workstation Playbook_ is free and open source software.

[mit]: https://opensource.org/licenses/MIT
