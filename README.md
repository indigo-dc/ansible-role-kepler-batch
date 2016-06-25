Role and Dockerfile for Kepler Workflow engine
==============================================

Roles and Dockerfiles to install the Kepler Workflow engine:

* To be updated

Introduction
------------

The repository contains ansible-roles that are published in
ansible galaxy:
* https://galaxy.ansible.com/indigo-dc/kepler/

The directory docker-kepler is linked to
dockerhub with automatic build. This image can run
the Kepler Workflow engine

Requirements
------------

No aditional requirements

Role Variables
--------------

The variables that can be passed to this role and a brief description
about them are as follows.

Dependencies
------------

None for now

Install the Playbook
--------------------

To install the role:

```
$ ansible-galaxy install indigo-dc.kepler
```

Run the playbook
----------------

An example of playbook for the kepler:

```
---
- hosts: localhost
  remote_user: root
  roles:
    - indigo-dc.kepler
```

Or execute:

```
$ ansible-playbook /etc/ansible/roles/indigo-dc.kepler/tests/kepler.yml
```

Run the kepler workflow application
-----------------------------------

To be updated

License
-------

Apache v2

Author Information
------------------

Mario David: mariojmdavid@gmail.com
LIP and Indigo-DataCloud project

Acknowledgments
---------------

* Kepler and Kepler WF for Indigo