# Ansible Role: Ghost

## Requirements

Requires Node.js (via the NodeSource PPA).

## Role Variables

Available variables are listed below, along with their default values:

    ghost_user: ghost
    ghost_user_home: /home/ghost

The user and home under which Ghost will be run and installed.

    ghost_binary_url: https://ghost.org/zip/ghost-0.5.3.zip

Download URL for the Ghost zip.

    ghost_http_port: "5000"

HTTP port over which Ghost will be accessed.

## Dependencies

None.

## Example Playbook

    - hosts: servers
      vars_files:
        - vars/main.yml

*Inside `vars/main.yml`*:

    ghost_http_port: "80"

## License

MIT

## Author Information

This role was created in 2014 by [Adel Qalieh](https://github.com/adelq/).
