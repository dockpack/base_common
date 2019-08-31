[![Galaxy](https://img.shields.io/badge/galaxy-dockpack.base__common-blue.svg?style=flat)](https://galaxy.ansible.com/dockpack/base_common)[![Build Status](https://api.travis-ci.org/dockpack/base_common.svg)](https://travis-ci.org/dockpack/base_common)

base_common is a role that provisions sensible defaults for Centos 7

Requirements
------------

RHEL- like system


Role Variables
--------------

server:
    install: true
    packages: 
      - postfix

Dependencies
------------

base_common is a role that other base roles can depend on.

Example Usage
----------------

Refer to a complete build server https://github.com/bbaassssiiee/buildserver

License
-------

MIT

Author Information
------------------

Bas Meijer
@bbaassssiiee
