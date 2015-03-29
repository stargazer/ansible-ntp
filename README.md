# ansible-ntp

This Ansible role makes sure that any remote Debian server has the correct local time.

## Role Variables

``timezone``: Default is ``Europe/Amsterdam``

## Examples

``playbook.yml``

        ---
        hosts: all
        remote_user: foo
        sudo: yes
        roles:
         - {role: 'ansible-ntp', timezone: "Europe/Amsterdam"}

Invoke playbook

        ansible-playbook playbook.yml

