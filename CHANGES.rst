Changelog
=========

v0.2.0
------

*Unreleased*

- Add Changelog. [ypid]

- Use ``debops.mariadb`` to allow to use MariaDB or MySQL on a remote server. [ypid]

- Updated to ownCloud 8.1. [ypid]

- Allow to use ``ooc`` via Ansible’s inventory. Can be used to enable apps and create users. [ypid]

- Setup shortcut for the `occ` command when not logged in as ``owncloud_user`` user and sudo allows it.
  Disabled by default. Can be enabled via ``owncloud_enable_occ_shortcut``. [ypid]

- Improved LDAP support. Now role will create service account (default: ``cn=owncloud,dc=ansible,dc=fqdn``)
  in ldap server. You still have to provied proper permission for this account. [scibi]

- New PostgreSQL role support. Now PostgreSQL and MariaDB/MySQL support is unified. [scibi]

- New variable: ``owncloud_timeout`` needed to handle very large files uploads. [scibi]
