Docker-Transmission
=========

Ansible role to deploy linuxserver/transmission docker container 

Requirements
------------

* Ansible >= 2.9
* geerlinguy.docker role <https://galaxy.ansible.com/geerlingguy/docker>

Role Variables
--------------

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
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: docker-transmission, __tranmission_defaut_TZ: Europe/London }

License
-------

BSD

Author Information
------------------

christophepiv@gmail.com
