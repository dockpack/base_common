=========

base_common is a role that other base roles depend on.

Requirements
------------

RHEL- like system


Role Variables
--------------

server:
    install: '1'
    packages: [ca-certificates]
    locale: en_US.UTF-8

Dependencies
------------

base_common is a role that other base roles depend on.

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
