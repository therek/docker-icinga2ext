# What is icinga2ext

[![Docker Automated Build](https://img.shields.io/docker/automated/jrottenberg/ffmpeg.svg)](https://img.shields.io/docker/automated/jrottenberg/ffmpeg.svg)
[![Docker Build Status](https://img.shields.io/docker/build/jrottenberg/ffmpeg.svg)](https://img.shields.io/docker/build/jrottenberg/ffmpeg.svg)

This repository contains the source for the [Icinga2](https://www.icinga.org/icinga2/) [Docker](https://www.docker.com) image.

It is based heavily on Jordan Jethwa's [Icinga2 Docker image](https://github.com/jjethwa/icinga2) with some additions:
* added `nslookup` and `dig` commands for `check_dns` and `check_dig` plugins;
* added `whois` command;
* added Net::SNMP Perl module for SNMP Manubulon plugins.

For container configuration please see [jordan/icinga2](https://hub.docker.com/r/jordan/icinga2/).

## Usage

Start a new container and bind to host's port 80

    docker run -p 80:80 -t therek/icinga2ext:latest
