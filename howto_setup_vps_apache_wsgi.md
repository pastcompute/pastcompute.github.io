---
layout: page
title: Configure a VPS for rapid web prototyping using Apache &amp; a Python WSGI framework
permalink: /howto_setup_vps_apache_wsgi/
---

# Configure a VPS for rapid web prototyping using Apache &amp; a Python WSGI framework

This page describes how to setup a new Linux VPS to serve Python WSGI applications.

This is likely to be useful when rapid prototyping during a hackathon such as [Unleashed](http://uladl.com)/[GovHack](http://www.govhack.org)

See also: notes about bringing up an AWS VPS

See also: notes about bringing up a VULTR VPS

## Notes

* assumes Ubuntu server 14.04 LTS
* add extra packages as needed
* not all of the packages list here may be needed, but I used them in varying combinations across multiple hackathons

## Procedures

The following commands are all done as root. Add `sudo` as required by your security policies.

### Install Packages

    apt-get update
    apt-get install postgresql-9.3-postgis-2.1 apache2 git vim php5 unzip libapache2-mod-python pgadmin3 python-psycopg2
    apt-get install python-setuptools libapache2-mod-wsgi
    easy_install web.py

(Note that on some O/S versions it may be necessary to do `service apache2 restart`)

### Configure Apache2


