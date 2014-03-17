jmartin.collectd
========

Configures collectd

Requirements
------------

These modules require collected 5.3 or later.

Role Variables
--------------


| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
|collectd_bind_ip| 0.0.0.0 | Collectd Server IP address to bind to |
|collectd_graphite_addr | 127.0.0.1 | address of graphite server |
|collectd_graphite_port  | 2003| port of graphite server |
| collectd_hostname | {{ ansible_fqdn }} | hostname to use for agent  |
| collectd_iface | eth0 | interface that collectd server will bind to |
| collectd_fqdnlookup | no | allow collectd to detect fqdn |
| collectd_typesdb | no | use a custom types db |
| collectd_interval | 10 | number of seconds between value collections |
| collectd_timeout | 2 | number of seconds to wait before agent timeout |
| collectd_threads | 5 | number of working collectd threads | 
|riak_http_port | 8098 | If using Riak, the default port to listen |
| riakcs_port | 8080   | If using Riak CS, the default port to listen |

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
-------------------------

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
