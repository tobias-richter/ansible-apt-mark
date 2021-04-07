# tobias_richter.apt_mark

[![Build Status](https://github.com/tobias-richter/ansible-apt-mark/workflows/CI/badge.svg)](https://github.com/tobias-richter/ansible-apt-mark/actions)

This role supports marking APT packages as `hold` and `unhold`

## Requirements

This role requires Ansible 2.7 or higher.

## Role Variables

See [defaults/main.yml](defaults/main.yml) for the documented role variables.

## Example Playbook

This playbook creates a user named john_doe with no password and the primary group john_doe.

    - hosts: debian
	  roles:
	    - role: tobias_richter.apt_mark
          apt_mark_hold_packages:
            - jenkins      
