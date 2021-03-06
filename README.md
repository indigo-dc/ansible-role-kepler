[![License](http://img.shields.io/:license-apache-blue.svg?style=flat-square)](http://www.apache.org/licenses/LICENSE-2.0.html)
[![Build Status](https://travis-ci.org/indigo-dc/ansible-role-kepler.svg?branch=master)](https://travis-ci.org/indigo-dc/ansible-role-kepler)

Role and Dockerfile for Kepler Workflow engine
==============================================

Roles and Dockerfiles to install the Kepler Workflow engine:

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

* indigo_kepler_version: a version of indigo-dc/indigokepler module to be used
* password_vnc: password to connect to VNC

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
  become: true
  roles:
    - indigo-dc.kepler
```

Or execute:

```
$ ansible-playbook /etc/ansible/roles/indigo-dc.kepler/tests/kepler.yml
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
