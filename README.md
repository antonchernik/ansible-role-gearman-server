Gearmand server
=========

Gearmand role for installing Gearmand server. Tested platforms are:
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
| gearmand_tarball_url  | yes | https://launchpad.net/gearmand/1.2/1.1.12/+download/gearmand-1.1.12.tar.gz | | Sets Gearmand tarball url  |
| gearmand_tarball_directory | yes  | gearmand-1.1.12 | | Sets Gearmand extract directory |
| gearmand_user_name | yes  | gearmand | | Sets Gearmand system user to run with /sbin/nologin |


Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
