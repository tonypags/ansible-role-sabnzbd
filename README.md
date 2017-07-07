ansible-role-sabnzbd
=========

An Ansible role to install SABnzbd on CentOS 7

Requirements
------------

- CentOS/Red Hat Enterprise Linux 7 

Role Variables
--------------

Defaults:

- sabnzbd_directory = /opt/sabnzbd/ - directory to clone the sabnzbd repo to
- sabnzbd_user = usenet - user that will run sabnzbd

Vars:

- rpmforge_repo - url to the rpmforge repo RPM package, required for the non-free unrar package
- sabnzbd_prereqs - all the sabnzbd prerequisite packages that need to be installed via Yum
- pip_prereqs - all the pip prerequisite packages that need to be installed via pip

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: mujahidhemani.sabnzbd }

License
-------

GPLv3

Author Information
------------------

Author: Mujahid Hemani
