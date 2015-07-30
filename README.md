Observium
=========

[Observium](http://observium.org) is a low-maintenance auto-discovering network monitoring platform supporting a wide range of device types, platforms and operating systems including Cisco, Windows, Linux, HP, Juniper, Dell, FreeBSD, Brocade, Netscaler, NetApp and many more. Observium focuses on providing a beautiful and powerful yet simple and intuitive interface to the health and status of your network.

Requirements
------------

- MySQL
- Apache
- Ports 80 and 443 open in the firewall

Role Variables
--------------

|   Name       | Default Value | Description                    |
|--------------|---------------|--------------------------------|
| `ob_var1`    | foo           | bar                            |



Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

MIT
