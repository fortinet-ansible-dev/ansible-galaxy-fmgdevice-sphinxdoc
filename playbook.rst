
Run Your First Playbook
==============================

This document explains how to run your first FortiManager Device Ansible playbook.

--------------

With FortiManager Device Galaxy collection, you are always recommended to run
FortiManager Device module in ``httpapi`` manner. The first step is to prepare your
host inventory with which you can use ``ansible-vault`` to encrypt or
decrypt your secrets for the sake of confidentiality.

Prepare host inventory
~~~~~~~~~~~~~~~~~~~~~~

In our case we create a file named ``hosts``:
This file specifies one FortiManager instance and some variables the instance are using.

With Standard User/password authentication
----------

::

   [fortimanagers]
   # Storing authentication token in plain text file is a bad idea on a security point of view
   # Please prefer ansible-vault or any encrypted mean to store sensitive data
   fortimanager01 ansible_host=192.168.190.1 ansible_user="admin" ansible_password="password"
   fortimanager02 ansible_host=192.168.190.2 ansible_user="admin" ansible_password="password"

   [fortimanagers:vars]
   ansible_connection=httpapi
   ansible_network_os=fortinet.fmgdevice.fmgdevice
   ansible_facts_modules=setup
   ansible_httpapi_port=443
   ansible_httpapi_use_ssl=true
   #  Disabling TLS certificate verification is a bad idea on security point of view, 
   #  but if you use default certificates that are self-signed, you need to disable it.
   #  Please use valid certificates for your production environments and keep certificate validation ON.
   ansible_httpapi_validate_certs=false

With REST API user token based authentication
----------

::

   [fortimanagers]
   # Storing authentication token in plain text file is a bad idea on a security point of view
   # Please prefer ansible-vault or any encrypted mean to store sensitive data
   fortimanager01 ansible_host=192.168.190.1 api_bearer_token="YOUR_GENERATED_API_KEY"
   fortimanager02 ansible_host=192.168.190.2 api_bearer_token="YOUR_GENERATED_API_KEY"

   [fortimanagers:vars]
   ansible_connection=httpapi
   ansible_network_os=fortinet.fmgdevice.fmgdevice
   ansible_facts_modules=setup
   ansible_httpapi_port=443
   ansible_httpapi_use_ssl=true
   #  Disabling TLS certificate verification is a bad idea on security point of view, 
   #  but if you use default certificates that are self-signed, you need to disable it.
   #  Please use valid certificates for your production environments and keep certificate validation ON.
   ansible_httpapi_validate_certs=false
  

Write the playbook
~~~~~~~~~~~~~~~~~~

An Example with User/Password authentication
----------

Create the file ``test.yml``:

::

  - name: Gathering fortimanager facts
    hosts: fortimanagers
    connection: httpapi
    vars:
      device_name: "XXXXXXX"
      vdom_name: "root"
    tasks:
      - name: Gathering fortimanager fact
        fortinet.fmgdevice.fmgd_fact:
          facts:
            selector: "alertemail_setting"
            params:
              device: "{{ device_name }}"
              vdom: "{{ vdom_name }}"
        register: response
      - name: Display response
        debug:
          var: response


An Example with REST API user token based authentication
----------

Create the file ``test.yml``:

::

  - name: Gathering fortimanager facts
    hosts: fortimanagers
    connection: httpapi
    vars:
      ansible_httpapi_session_key:
        authorization: "bearer {{ api_bearer_token }}"
      device_name: "XXXXXXX"
      vdom_name: "root"
    tasks:
      - name: Gathering fortimanager fact
        fortinet.fmgdevice.fmgd_fact:
          facts:
            selector: "alertemail_setting"
            params:
              device: "{{ device_name }}"
              vdom: "{{ vdom_name }}"
        register: response
      - name: Display response
        debug:
          var: response


Parameter Usages
----------------

For details about how to use modules, please check:

- `Device modules page`_ Modules that releated with FortiManager Device.
- `fmgd_fact`_ Gather FortiManager Device Facts.
- `fmgd_rename`_ Rename an object in FortiManager.
- `fmgd_clone`_ Clone an object in FortiManager.
- `fmgd_move`_ Move fortimanager defined Object.
- `fmgd_generic`_ The Generic FortiManager module.

.. _Device modules page: modules.html
.. _fmgd_fact: fmgd_fact.html
.. _fmgd_rename: fmgd_rename.html
.. _fmgd_clone: fmgd_clone.html
.. _fmgd_move: fmgd_move.html
.. _fmgd_generic: fmgd_generic.html

Run the playbook
~~~~~~~~~~~~~~~~

::

   ansible-playbook -i hosts test.yml

you can also observe the verbose output by adding option at the tail:
``-vvv``.
