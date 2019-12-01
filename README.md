Firewalld
=========

This role started out as an experiment to get Firewalld running
on Debian 10, but it turned out to be a failure.

Installs and tries to configure Firewalld.

Turns out firewalld doesn't work properly on Debian 10 due to
missing dependency of python3-firewall(python3-firewall.noarch : Python3 bindings for firewalld).

Requirements
------------

None.

Role Variables
--------------

There are are some examples found in [defaults/main.yml](../defaults/main.yml), but by
default the role doesn't configure anything, just installs Firewalld.

Dependencies
------------


[Requirements from ansible docs/firewalld](https://docs.ansible.com/ansible/latest/modules/firewalld_module.html)

The below requirements are needed on the host that executes this module.

firewalld >= 0.2.11

Versions in this release:

[Debian search result for firewalld as of 2019-11-30](https://packages.debian.org/search?keywords=firewalld)


- jessie (oldoldstable) (net): 0.3.12-1: all
- stretch (old stable) (net): 0.4.4.2-1: all
- buster (stable) (net): 0.6.3-5: all
- bullseye (testing) (net): 0.7.2-1: all
- sid (unstable) (net): - 0.7.2-1: all

License
-------

GPLv3

Author Information
------------------

Richard Skumat
