=====
acme
=====

description
============

works with Ubuntu 14.04/18.04

this role sets up LetsEncrypt on a server

this role can deploy 2 different agents:

- a minimal "acme_tiny" script and helper tool that has minimal dependencies
- the standard "certbot" tool endorsed by LetsEncrypt

usage
======

fill in the variables presented in defaults/main.yml

multiple domains can be declared per server

acme_tiny
----------

this role depends on acme_tiny_ and acme_tiny_renew_ (note that this role does not provide a way to fetch/update these, they must be provided separately)

certbot
--------

this role depends on certbot_ (which is installed by the role)



.. _certbot: https://launchpad.net/~certbot/+archive/ubuntu/certbot
.. _acme_tiny: https://github.com/diafygi/acme-tiny/
.. _acme_tiny_renew: https://github.com/gitgruub/acme-tiny-renew/
