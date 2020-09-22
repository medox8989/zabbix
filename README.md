Ansible role for Odoo in docker
===============================

Create and deploy an odoo instance though docker containers. Two containers are created and managed though a docker-compose file :
- one for Odoo;
- one for the database (Postgres).

Role Variable
=============

Expected to be configured
-------------------------

- `odoo_db_user`: Username to use for the Postgres database
- `odoo_db_password`: Password to use for the Postgres database

Optionnals
----------

- `odoo_version` (default: 10): Version of Odoo to deploy, this is the [tag name](https://hub.docker.com/r/library/odoo/tags/) of the docker image
- `odoo_app_path` (default: /srv/odoo): The path where all files (such as docker-compose file) are located
