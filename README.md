freehck.pip_install
=========

Install pip packages.



Description
-----------

This role simply installs a list of pip packages.

As it's a pip module wrapped into role, you can use it as a dependency in other role's meta.

Role Variables
--------------

`pip_install_packages`: list of packages to install

`pip_install_state`: state of package

It can be `present` (default), `latest` or `absent`

Example
-------

    - hosts: all
      become: true
      roles:
        - role: freehck.pip_install
          pip_install_packages:
            - docker

Install
-------

This role can be installed from [Ansible Galaxy](https://galaxy.ansible.com/):

`ansible-galaxy install freehck.pip_install`

License
-------

MIT

Author Information
------------------

Dmitrii Kashin, <freehck@freehck.ru>
