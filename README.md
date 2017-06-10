Gearman server
=========

Gearman role for installing Gearman server. Tested platforms are:
* Debian 8

Requirements
------------

Debian 8 (jessie)

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

| Parameter | Required | Default | Choices | Comments |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| default_download_directory | yes | /tmp | | Sets directory where files will be downloaded |
| gearmand_tarball_url  | yes | https://launchpad.net/gearmand/1.2/1.1.12/+download/gearmand-1.1.12.tar.gz | | Sets Gearman server tarball url  |
| gearmand_tarball_directory | yes  | gearmand-1.1.12 | | Sets Gearman extract directory |
| gearmand_user_name | yes  | gearmand | | Sets Gearman system user to run with /sbin/nologin |


Dependencies
------------

None

Example 
----------------
    ---
    - hosts: all
      roles:
         - { role: antonchernik.gearman-server }

License
-------

MIT / BSD

Author Information
------------------

This role was created in 2017 by [Anton Chernik](https://github.com/antonchernik).
