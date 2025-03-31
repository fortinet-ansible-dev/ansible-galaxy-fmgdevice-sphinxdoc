FortiManager Best Practices
====================================

FortiManager is an integrated platform for the centralized management of products in a Fortinet security infrastructure, including FortiGates.

FortiManager has two separate Ansible Collections:

- `FortiManager Ansible Collection`_ is used to configure settings in FortiManager.
- `FortiManager Device Ansible Collection`_ is used to configure the devices managed by the FortiManager.

Once FortiGates are managed by a FortiManager that is operating in Normal Mode, whenever possible, configuration changes should be made on the FortiManager and not the FortiGate. This recommendation also applies when the configuration of FortiGates and FortiManager is executed through 
the `FortiOS Ansible Collection`_, `FortiManager Ansible Collection`_ and `FortiManager Device Ansible Collection`_ collections.

To help you get the most out of your FortiManager products, maximize performance, and avoid potential problems, please refer to the `FortiManager documentation`_, including the Administration Guide and Best Practices documents.

Fortinet also provides a developer community to help administrators and advanced users enhance and increase the effectiveness of Fortinet products. The `Fortinet Developer Network (FNDN)`_ provides the official documentation and advanced tools for developing custom solutions using Fortinet products.



.. _FortiOS Ansible Collection: https://ansible-galaxy-fortios-docs.readthedocs.io/en/latest/
.. _FortiManager Ansible Collection: https://ansible-galaxy-fortimanager-docs.readthedocs.io/en/latest/
.. _FortiManager Device Ansible Collection: https://ansible-galaxy-fmgdevice-docs.readthedocs.io/en/latest/
.. _FortiManager documentation: https://docs.fortinet.com/product/fortimanager
.. _Fortinet Developer Network (FNDN): https://fndn.fortinet.net/

