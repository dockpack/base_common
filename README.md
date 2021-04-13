[![Galaxy](https://img.shields.io/badge/galaxy-dockpack.base__common-blue.svg?style=flat)](https://galaxy.ansible.com/dockpack/base_common)

base_common is a role that provisions sensible defaults for Centos 7.

- The openssh-server is hardened to [ssh-audit standards](https://www.ssh-audit.com/hardening_guides.html).
- This config removes the [deprecated ssh-rsa host key](https://www.openssh.com/txt/release-8.2)

Requirements
------------

RHEL- like system


Role Variables
--------------

```
server:
  install: true
  packages:
    - policycoreutils-python
    - libsemanage-python
    - postfix
# sshd
Ciphers: chacha20-poly1305@openssh.com,aes256-gcm@openssh.com,aes128-gcm@openssh.com,aes256-ctr,aes192-ctr,aes128-ctr
HostKeyAlgorithms: ssh-ed25519-cert-v01@openssh.com,ssh-ed25519
KexAlgorithms: curve25519-sha256@libssh.org,diffie-hellman-group18-sha512,diffie-hellman-group16-sha512,diffie-hellman-group14-sha256
MACs: hmac-sha2-256-etm@openssh.com,hmac-sha2-512-etm@openssh.com,umac-128-etm@openssh.com
```


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
