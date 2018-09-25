cisco-conference-room-endpoint-config
=========

Returns the Cisco Configuration Room Endpoint Configuration.

Returns the Cookie Session ID used for amending the configuration of the Cisco
Conference room Endpoint.

Supports the following Cisco Endpoints

* Blah Blah
* Blah Blah

Requirements
------------

* Ansible 2.5. Requires the ``parse_xml`` filter.

Role Variables
--------------

* ``url_protocol``: Can be either ``https`` or ``http``. By default it is ``https``
* ``conf_endpoint_config``: XML configuration of the Cisco Conf Room Endpoint

Dependencies
------------

N/A


Example Playbook
----------------

```

- hosts: cisco_endpoints
  connection: local
  gather_facts: no
  tasks:
    - name: Print the list of inaccessible hosts (send to Slack or Mail in production)
      debug:
        var: inaccessible_hosts
  roles:
     - { role: cisco-conf-room-endpoint-config}
     - { role: cisco-convert-from-h323-to-sip}

```


License
-------

MIT

Author Information
------------------

Stanley Karunditu
@linuxsimba
