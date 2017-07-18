# icinga2ext

This repository contains the source for the
[Icinga2](https://www.icinga.org/icinga2/) [Docker](https://www.docker.com)
image.

It is based heavily on Jordan Jethwa's Icinga2 Docker image with some additions:
* added `nslookup` and `dig` for `check_dns` and `check_dig` plugins;
* added Net::SNMP Perl module for SNMP Manubolon plugins.

For container configuration please see
[jordan/icinga2](https://hub.docker.com/r/jordan/icinga2/).
