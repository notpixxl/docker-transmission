Docker-Transmission
=========

Ansible role to install linuxserver/transmission docker container

Requirements
------------

* Ansible >= 2.9
* geerlinguy.docker role <https://galaxy.ansible.com/geerlingguy/docker>

Role Variables
--------------

Ansible variables are listed below with their default values.

```yaml
__transmission_default_user: transmission #Best supersed it on vault file
__transmission_default_pass: transmission #Best supersed it on vault file
__transmission_default_TZ: Europe/Paris
__transmission_default_config_path: ~/transmission/config/
__transmission_default_download_path: ~/transmission/download/
__transmission_default_watch_path: ~/transmission/watch/
__transmission_default_webinterface_port: 9091
```

Dependencies
------------

None

Example Playbook
----------------`

```yaml
- hosts: servers
  roles:
     - { role: notpixxl.docker_transmission, __tranmission_default_TZ: Europe/London }
```

License
-------

BSD

Author Information
------------------

christophepiv@gmail.com
