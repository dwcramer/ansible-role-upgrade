# Ansible Role: Upgrade

[![MIT License](http://img.shields.io/badge/license-MIT-003399.svg)](http://opensource.org/licenses/MIT)

An Ansible role that upgrades installed packages on Ubuntu 14.04

## Requirements

None

## Role Variables

Ansible variables are listed here along with their default values:

`upgrade_update_grub` flags whether or not to run `update-grub` after
`autoremove`.

    upgrade_update_grub: true

## Dependencies

None

## Example Playbook

    ---
    - hosts: all
      vars:
      - upgrade_update_grub: false
      roles:
      - novuso.upgrade

## License

This is released under the [MIT license](http://opensource.org/licenses/MIT).
