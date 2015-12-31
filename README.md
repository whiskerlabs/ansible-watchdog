# armsible-watchdog

[![Ansible Galaxy](http://img.shields.io/badge/galaxy-whiskerlabs.watchdog-660198.svg)](https://galaxy.ansible.com/list#/roles/6649)

An Ansible role for installing and configuring the
[software watchdog daemon provided by the Linux kernel](http://linux.die.net/man/8/watchdog).

This role installs the `watchdog` apt package and configures
`/etc/watchdog.conf` according to values defined in
`defaults/main.yml`.

## Installation

To install from Ansible Galaxy:

    $ ansible-galaxy install whiskerlabs.watchdog

Or alternatively, add the path to a local copy of this repository to
`roles_path` within your project's `ansible.cfg` file:

    roles_path = /path/to/role_dir

where `/path/to/role_dir` is a parent directory of
`armsible-watchdog`.

Consult
[Ansible documentation](http://docs.ansible.com/intro_configuration.html)
for more info on how to configure `roles_path` in an Ansible
configuration file.

## Requirements

Target hosts must be Linux machines running a Debian-based distro. The
only reason for this is because apt is currently used to install the
`watchdog` package.

`armsible-watchdog` has no role dependencies.

## Role Variables

See documentation in `defaults/main.yml`.

## License

Copyright 2016 Whisker Labs

Licensed under the MIT License. See `LICENSE` for details.
