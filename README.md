# ansible-digital-rebar

An [Ansible](https://www.ansible.com) role to install/configure [Digital Rebar](http://rebar.digital/)

## Requirements

## Role Variables

Default configuration variables

```
digital_rebar_version: 3.13.4
digital_rebar_installer_sha256: 9d0e150865b8b4db2d0aae2cb0686254e95b8a976e36de5604b8a3f9c95de3c7
```

Additional var/main.yml derived / static values.

```
digital_rebar_binary: "{{ digital_rebar_install_dir }}/dr-provision"
digital_rebar_installer_url: https://raw.githubusercontent.com/digitalrebar/provision/{{ digital_rebar_version }}/tools/install.sh
digital_rebar_install_dir: /usr/local/bin
```

## Dependencies

## Example Playbook

```
---
- hosts: bastion
  roles:
    - { role: neutron37.ansible-digital-rebar-multiplatform }
```

## License

MIT

## Author Information

Tom Stec

- tom [at] satori.us

Forked from mrlesmithjr/ansible-digital-rebar
Original author: Larry Smith Jr.

-   [EverythingShouldBeVirtual](http://everythingshouldbevirtual.com)
-   [@mrlesmithjr](https://www.twitter.com/mrlesmithjr)
-   mrlesmithjr [at] gmail.com

