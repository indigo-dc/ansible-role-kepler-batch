[![License](http://img.shields.io/:license-apache-blue.svg?style=flat-square)](http://www.apache.org/licenses/LICENSE-2.0.html)
[![Build Status](https://travis-ci.org/indigo-dc/ansible-role-kepler.svg?branch=master)](https://travis-ci.org/indigo-dc/ansible-role-kepler)

Role and Dockerfile for Kepler Workflow engine
==============================================

Roles and Dockerfiles to install the Kepler Workflow engine:

Introduction
------------

The repository contains ansible-roles that are published in ansible galaxy:
* https://galaxy.ansible.com/indigo-dc/kepler-batch/

The directory docker-kepler is linked to dockerhub with automatic build. This image can run the Kepler Workflow engine

Requirements
------------

No aditional requirements

Role Variables
--------------

The variables that can be passed to this role and a brief description
about them are as follows.

* futuregateway_uri: URI to a running FutureGateway instance
* authorization_token: auth token, useful only for short debugging sessions
* indigo_kepler_version: a version of indigo-dc/indigokepler module to be used

Dependencies
------------

None for now

Install the Playbook
--------------------

To install the role:

```
$ ansible-galaxy install indigo-dc.kepler-batch
```

Run the playbook
----------------

An example of playbook for the kepler:

```
---
- hosts: localhost
  become: true
  roles:
    - indigo-dc.kepler-batch
```

Or execute:

```
$ ansible-playbook /etc/ansible/roles/indigo-dc.kepler-batch/tests/kepler.yml
```

Run the kepler workflow application
-----------------------------------

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
