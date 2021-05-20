Ansible Role: Veritas NetBackup client
=========

Ansible role to install [Veritas NetBackup](https://www.veritas.com/protection/netbackup) client on Linux Servers.

Requirements
------------

The role does not require anyting to run on RHEL and its derivatives.

Role Variables
--------------

Available variables are listed below, along with default values ```(see defaults/main.yml)```:

``` yaml
software_url: "http://www.example.org"
package_name: "netbackup-client.zip"
```

```software_url``` **(Required)** The URL that hosts the Installer package. This should be either **http** or **https**.

```package_name``` **(Required)** The Installer package name.

Role variables can be stored with the hosts.yaml file, or in the main variables file.

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

``` yaml
    - hosts: servers
      roles:
         - role: mikepruett3.netbackup-client
           vars:
             software_url: "http://www.example.org"
             package_name: "netbackup-client.zip"
```

License
-------

MIT

Author Information
------------------

Role created by [mikepruett3](https://github.com/mikepruett3) on [Github.com](https://github.com/mikepruett3)
