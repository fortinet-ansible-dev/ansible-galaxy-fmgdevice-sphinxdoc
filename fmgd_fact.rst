:source: fmgd_fact.py

:orphan:

.. _fmgd_fact:

fmgd_fact -- Gather FortiManager Device Facts.
++++++++++++++++++++++++++++++++++++++++++++++

.. versionadded:: 1.0.0

.. contents::
   :local:
   :depth: 1


Synopsis
--------

- This module is able to configure a FortiManager device.
- Examples include all parameters and values need to be adjusted to data sources before usage.
- Tested with FortiManager v7.x.


Requirements
------------
The below requirements are needed on the host that executes this module.

- ansible>=2.15.0



Parameters
----------

.. raw:: html

  <ul>
  <li><span class="li-head">access_token</span> -The token to access FortiManager without using username and password. <span class="li-normal">type: str</span> <span class="li-required">required: false</span></li>
  <li><span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal"> default: False</span> </li>
  <li><span class="li-head">forticloud_access_token</span> - Access token of forticloud managed API users, this option is available with FortiManager later than 6.4.0. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
  <li><span class="li-head">workspace_locking_adom</span> - Acquire the workspace lock if FortiManager is running in workspace mode. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal"> choices: global, custom adom including root</span> </li>
  <li><span class="li-head">workspace_locking_timeout</span> - The maximum time in seconds to wait for other users to release workspace lock. <span class="li-normal">type: integer</span> <span class="li-required">required: false</span>  <span class="li-normal">default: 300</span> </li>
  <li><span class="li-head">rc_succeeded</span> - The rc codes list with which the conditions to succeed will be overriden. <span class="li-normal">type: list</span> <span class="li-required">required: false</span> </li>
  <li><span class="li-head">rc_failed</span> - The rc codes list with which the conditions to fail will be overriden. <span class="li-normal">type: list</span> <span class="li-required">required: false</span> </li>

  <li><span class="li-head">facts</span> - Gathering fortimanager facts. <span class="li-normal">type: dict</span></li>
  <ul class="ul-self">
  <li><span class="li-head">selector</span> - Selector of the retrieved fortimanager facts. <span class="li-normal">type: str</span> <span class="li-required">choices:</span></li>
  <li style="list-style: none;"><section class="accordion">
  <input type="checkbox" name="collapse" id="handle2">
  <h2 class="handle">
      <label for="handle2"><u>Show full selector list...</u></label>
  </h2>
  <div class="content">
  <ul class="ul-self">
      <li><span class="li-required">alertemail_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">antivirus_exemptlist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">antivirus_heuristic</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">antivirus_quarantine</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">antivirus_settings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">application_name</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">application_rulesettings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">automation_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">aws_vpce</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">azure_vwaningresspublicips</span> - available versions:
          <span class="li-normal">v7.4.4->latest</span>
      </li>
      <li><span class="li-required">azure_vwanslb</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">azure_vwanslb_permanentsecurityrules</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">azure_vwanslb_permanentsecurityrules_rules</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">azure_vwanslb_temporarysecurityrules</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">azure_vwanslb_temporarysecurityrules_rules</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">casb_attributematch</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">casb_attributematch_attribute</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">certificate_remote</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">dlp_exactdatamatch</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">dlp_exactdatamatch_columns</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">dlp_fpdocsource</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">dlp_settings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">dpdk_cpus</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">dpdk_global</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">emailfilter_fortiguard</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">endpointcontrol_fctemsoverride</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">endpointcontrol_settings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">ethernetoam_cfm</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">ethernetoam_cfm_service</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">extendercontroller_extender</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">extendercontroller_extender_controllerreport</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">extendercontroller_extender_modem1</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">extendercontroller_extender_modem1_autoswitch</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">extendercontroller_extender_modem2</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">extendercontroller_extender_modem2_autoswitch</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">extendercontroller_extender_wanextension</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">extensioncontroller_extender</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">extensioncontroller_extender_wanextension</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">extensioncontroller_extendervap</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">extensioncontroller_fortigate</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">extensioncontroller_fortigateprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">extensioncontroller_fortigateprofile_lanextension</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_accessproxysshclientcert</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>
      </li>
      <li><span class="li-required">firewall_accessproxysshclientcert_certextension</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>
      </li>
      <li><span class="li-required">firewall_authportal</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_dnstranslation</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_global</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_internetserviceappend</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_internetservicedefinition</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_internetservicedefinition_entry</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_internetservicedefinition_entry_portrange</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_internetserviceextension</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_internetserviceextension_disableentry</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_internetserviceextension_disableentry_ip6range</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_internetserviceextension_disableentry_iprange</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_internetserviceextension_disableentry_portrange</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_internetserviceextension_entry</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_internetserviceextension_entry_portrange</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_ipmacbinding_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_ipmacbinding_table</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_iptranslation</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_ipv6ehfilter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_ondemandsniffer</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_pfcp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_policy</span> - available versions:
          <span class="li-normal">v6.0.0->latest</span>
      </li>
      <li><span class="li-required">firewall_sniffer</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_sniffer_anomaly</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_ssh_hostkey</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_ssh_localkey</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_ssh_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_ssl_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_sslserver</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">firewall_ttlpolicy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">ftpproxy_explicit</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">gtp_apnshaper</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">gtp_ieallowlist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.8</span>,
          <span class="li-normal">v7.4.3->v7.6.1</span>
      </li>
      <li><span class="li-required">gtp_ieallowlist_entries</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.8</span>,
          <span class="li-normal">v7.4.3->v7.6.1</span>
      </li>
      <li><span class="li-required">gtp_rattimeoutprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">icap_profile</span> - available versions:
          <span class="li-normal">v6.0.0->latest</span>
      </li>
      <li><span class="li-required">icap_server</span> - available versions:
          <span class="li-normal">v6.0.0->latest</span>
      </li>
      <li><span class="li-required">icap_servergroup</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">icap_servergroup_serverlist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">ips_decoder</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">ips_decoder_parameter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">ips_global</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">ips_rule</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">ips_rulesettings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">ips_settings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">ips_tlsactiveprobe</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">loadbalance_flowrule</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">loadbalance_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">loadbalance_setting_workers</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">loadbalance_workergroup</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">log_azuresecuritycenter2_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_azuresecuritycenter2_filter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_azuresecuritycenter2_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_azuresecuritycenter2_setting_customfieldname</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_azuresecuritycenter_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_azuresecuritycenter_filter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_azuresecuritycenter_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_azuresecuritycenter_setting_customfieldname</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_disk_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_disk_filter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_disk_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_eventfilter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer2_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer2_filter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer2_overridefilter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer2_overridefilter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer2_overridesetting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer2_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer3_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer3_filter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer3_overridefilter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer3_overridefilter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer3_overridesetting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer3_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer_filter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer_overridefilter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer_overridefilter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer_overridesetting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzer_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzercloud_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzercloud_filter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzercloud_overridefilter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzercloud_overridefilter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzercloud_overridesetting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortianalyzercloud_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortiguard_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortiguard_filter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortiguard_overridefilter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortiguard_overridefilter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortiguard_overridesetting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_fortiguard_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_guidisplay</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_memory_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_memory_filter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_memory_globalsetting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_memory_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_nulldevice_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_nulldevice_filter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_nulldevice_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_slbc_globalsetting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd2_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd2_filter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd2_overridefilter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd2_overridefilter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd2_overridesetting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd2_overridesetting_customfieldname</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd2_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd2_setting_customfieldname</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd3_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd3_filter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd3_overridefilter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd3_overridefilter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd3_overridesetting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd3_overridesetting_customfieldname</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd3_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd3_setting_customfieldname</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd4_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd4_filter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd4_overridefilter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd4_overridefilter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd4_overridesetting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd4_overridesetting_customfieldname</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd4_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd4_setting_customfieldname</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd_filter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd_overridefilter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd_overridefilter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd_overridesetting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd_overridesetting_customfieldname</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_syslogd_setting_customfieldname</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_tacacsaccounting2_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_tacacsaccounting2_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_tacacsaccounting3_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_tacacsaccounting3_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_tacacsaccounting_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_tacacsaccounting_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_webtrends_filter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_webtrends_filter_freestyle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">log_webtrends_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">monitoring_np6ipsecengine</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">monitoring_npuhpe</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">notification</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">nsx_profile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">nsxt_servicechain</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">nsxt_servicechain_serviceindex</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">nsxt_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">pfcp_messagefilter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_chart</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_chart_categoryseries</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_chart_column</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_chart_column_mapping</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_chart_drilldowncharts</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_chart_valueseries</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_chart_xseries</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_chart_yseries</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_dataset</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_dataset_field</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_dataset_parameters</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_layout</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_layout_bodyitem</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_layout_bodyitem_list</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_layout_bodyitem_parameters</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_layout_page</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_layout_page_footer</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_layout_page_footer_footeritem</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_layout_page_header</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_layout_page_header_headeritem</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_style</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">report_theme</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_authpath</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bfd</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bfd6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bfd6_multihoptemplate</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bfd6_neighbor</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bfd_multihoptemplate</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bfd_neighbor</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_admindistance</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_aggregateaddress</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_aggregateaddress6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_neighbor</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_neighbor_conditionaladvertise</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_neighbor_conditionaladvertise6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_neighborgroup</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_neighborrange</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_neighborrange6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_network</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_network6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_redistribute</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_redistribute6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_vrf</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_vrf6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_vrf6_leaktarget</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_vrf_leaktarget</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_vrfleak</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_vrfleak6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_vrfleak6_target</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_bgp_vrfleak_target</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_extcommunitylist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_extcommunitylist_rule</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_isis</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_isis_isisinterface</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_isis_isisnet</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_isis_redistribute</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_isis_redistribute6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_isis_summaryaddress</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_isis_summaryaddress6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_keychain</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_keychain_key</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_multicast</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_multicast6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_multicast6_interface</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_multicast6_pimsmglobal</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_multicast6_pimsmglobal_rpaddress</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_multicast_interface</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_multicast_interface_igmp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_multicast_interface_joingroup</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_multicast_pimsmglobal</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_multicast_pimsmglobal_rpaddress</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_multicast_pimsmglobalvrf</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">router_multicast_pimsmglobalvrf_rpaddress</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">router_multicastflow</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_multicastflow_flows</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf6_area</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf6_area_ipseckeys</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf6_area_range</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf6_area_virtuallink</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf6_area_virtuallink_ipseckeys</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf6_ospf6interface</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf6_ospf6interface_ipseckeys</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf6_ospf6interface_neighbor</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf6_redistribute</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf6_summaryaddress</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf_area</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf_area_filterlist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf_area_range</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf_area_virtuallink</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf_area_virtuallink_md5keys</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf_distributelist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf_neighbor</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf_network</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf_ospfinterface</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf_ospfinterface_md5keys</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf_redistribute</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ospf_summaryaddress</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_policy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_policy6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_rip</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_rip_distance</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_rip_distributelist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_rip_interface</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_rip_neighbor</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_rip_network</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_rip_offsetlist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_rip_redistribute</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ripng</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ripng_aggregateaddress</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ripng_distance</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ripng_distributelist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ripng_interface</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ripng_neighbor</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ripng_network</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ripng_offsetlist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_ripng_redistribute</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_routemap</span> - available versions:
          <span class="li-normal">v7.0.2->latest</span>
      </li>
      <li><span class="li-required">router_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_static</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">router_static6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">rule_fmwp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">rule_otdt</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">rule_otvp</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_8021xsettings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_acl_group</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_acl_ingress</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_acl_ingress_action</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_acl_ingress_classifier</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_autoconfig_custom</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_autoconfig_custom_switchbinding</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_autoconfig_default</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_autoconfig_policy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_customcommand</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_dsl_policy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_dynamicportpolicy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_dynamicportpolicy_policy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_flowtracking</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_flowtracking_aggregates</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_flowtracking_collectors</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_fortilinksettings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_fortilinksettings_nacports</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_global</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_igmpsnooping</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_initialconfig_template</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_initialconfig_vlans</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_lldpprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_lldpprofile_customtlvs</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_lldpprofile_medlocationservice</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_lldpprofile_mednetworkpolicy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_lldpsettings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_location</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_location_addresscivic</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_location_coordinates</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_location_elinnumber</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_macpolicy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_8021xsettings</span> - available versions:
          <span class="li-normal">v6.0.0->v6.2.0</span>,
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_customcommand</span> - available versions:
          <span class="li-normal">v6.0.0->v6.2.0</span>,
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_dhcpsnoopingstaticclient</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_igmpsnooping</span> - available versions:
          <span class="li-normal">v6.0.0->v6.2.0</span>,
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_igmpsnooping_vlans</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_ipsourceguard</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_ipsourceguard_bindingentry</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_mirror</span> - available versions:
          <span class="li-normal">v6.0.0->v6.2.0</span>,
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_ports</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_ports_dhcpsnoopoption82override</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_remotelog</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_routeoffloadrouter</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_snmpcommunity</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_snmpcommunity_hosts</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_snmpsysinfo</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_snmptrapthreshold</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_snmpuser</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_staticmac</span> - available versions:
          <span class="li-normal">v6.2.0->v6.2.0</span>,
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_stormcontrol</span> - available versions:
          <span class="li-normal">v6.0.0->v6.2.0</span>,
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_stpinstance</span> - available versions:
          <span class="li-normal">v6.2.0->v6.2.0</span>,
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_stpsettings</span> - available versions:
          <span class="li-normal">v6.0.0->v6.2.0</span>,
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_switchlog</span> - available versions:
          <span class="li-normal">v6.0.0->v6.2.0</span>,
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_managedswitch_vlan</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_nacdevice</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_nacsettings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_networkmonitorsettings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_portpolicy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_ptp_interfacepolicy</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_ptp_policy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_ptp_profile</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_ptp_settings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_qos_dot1pmap</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_qos_ipdscpmap</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_qos_ipdscpmap_map</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_qos_qospolicy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_qos_queuepolicy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_qos_queuepolicy_cosqueue</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_remotelog</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_securitypolicy_8021x</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_securitypolicy_localaccess</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_sflow</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_snmpcommunity</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_snmpcommunity_hosts</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_snmpsysinfo</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_snmptrapthreshold</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_snmpuser</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_stormcontrol</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_stormcontrolpolicy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_stpinstance</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_stpsettings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_switchgroup</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_switchinterfacetag</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_switchlog</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_switchprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_system</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_trafficpolicy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_trafficsniffer</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_trafficsniffer_targetip</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_trafficsniffer_targetmac</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_trafficsniffer_targetport</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_virtualportpool</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">switchcontroller_vlanpolicy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_3gmodem_custom</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_5gmodem</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_5gmodem_dataplan</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_5gmodem_modem1</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_5gmodem_modem1_simswitch</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_5gmodem_modem2</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_accprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_accprofile_fwgrppermission</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_accprofile_loggrppermission</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_accprofile_netgrppermission</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_accprofile_sysgrppermission</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_accprofile_utmgrppermission</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_acme</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_acme_accounts</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_admin</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_affinityinterrupt</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_affinitypacketredistribution</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_alias</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_apiuser</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_apiuser_trusthost</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_arptable</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_autoinstall</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_automationaction</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_automationaction_httpheaders</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_automationcondition</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">system_automationdestination</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_automationstitch</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_automationstitch_actions</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_automationtrigger</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_automationtrigger_fields</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_autoscale</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_autoscript</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_autoupdate_pushupdate</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_autoupdate_schedule</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_autoupdate_tunneling</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_bypass</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_centralmanagement</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_centralmanagement_serverlist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_clustersync</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_clustersync_sessionsyncfilter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_clustersync_sessionsyncfilter_customservice</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_console</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_consoleserver</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_consoleserver_entries</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_csf</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_csf_fabricconnector</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_csf_fabricdevice</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_csf_trustedlist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ddns</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_dedicatedmgmt</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_deviceupgrade</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_deviceupgrade_knownhamembers</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_dhcp6_server</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_dhcp6_server_iprange</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_dhcp6_server_options</span> - available versions:
          <span class="li-normal">v7.6.0->latest</span>
      </li>
      <li><span class="li-required">system_dhcp6_server_prefixrange</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_digitalio</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_dnp3proxy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_dns</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_dns64</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_dnsdatabase</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_dnsdatabase_dnsentry</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_dnsserver</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_dscpbasedpriority</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_elbc</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_emailserver</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_evpn</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_fabricvpn</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_fabricvpn_advertisedsubnets</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_fabricvpn_overlays</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_federatedupgrade</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_federatedupgrade_knownhamembers</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_federatedupgrade_nodelist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_fipscc</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_fortiai</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_fortindr</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_fortisandbox</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_fssopolling</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ftmpush</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_geneve</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_gigk</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_global</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_gretunnel</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ha</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ha_frupsettings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ha_hamgmtinterfaces</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ha_secondaryvcluster</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ha_unicastpeers</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ha_vcluster</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_hamonitor</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_healthcheckfortiguard</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">system_icond</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup1</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup14</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup15</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup16</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup17</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup18</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup19</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup2</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup20</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup21</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup27</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup28</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup29</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup30</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup31</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup32</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ike_dhgroup5</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface_clientoptions</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface_dhcpsnoopingserverlist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface_egressqueues</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface_ipv6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface_ipv6_clientoptions</span> - available versions:
          <span class="li-normal">v7.6.0->latest</span>
      </li>
      <li><span class="li-required">system_interface_ipv6_dhcp6iapdlist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface_ipv6_ip6delegatedprefixlist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface_ipv6_ip6dnssllist</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">system_interface_ipv6_ip6extraaddr</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface_ipv6_ip6prefixlist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface_ipv6_ip6rdnsslist</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">system_interface_ipv6_ip6routelist</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">system_interface_ipv6_vrrp6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface_l2tpclientsettings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface_mirroringfilter</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface_secondaryip</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface_tagging</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface_vrrp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface_vrrp_proxyarp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_interface_wifinetworks</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ipam</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ipam_pools</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ipam_pools_exclude</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ipam_rules</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ipiptunnel</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ips</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ipsecaggregate</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ipsurlfilterdns</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ipsurlfilterdns6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ipv6neighborcache</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ipv6tunnel</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_iscsi</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_isfqueueprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_linkmonitor</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_linkmonitor_serverlist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_lldp_networkpolicy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_lldp_networkpolicy_guest</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_lldp_networkpolicy_guestvoicesignaling</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_lldp_networkpolicy_softphone</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_lldp_networkpolicy_streamingvideo</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_lldp_networkpolicy_videoconferencing</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_lldp_networkpolicy_videosignaling</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_lldp_networkpolicy_voice</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_lldp_networkpolicy_voicesignaling</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ltemodem</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ltemodem_dataplan</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ltemodem_simswitch</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_macaddresstable</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_memmgr</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_mobiletunnel</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_mobiletunnel_network</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_modem</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_nat64</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_nat64_secondaryprefix</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ndproxy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_netflow</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_netflow_collectors</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_netflow_exclusionfilters</span> - available versions:
          <span class="li-normal">v7.6.0->latest</span>
      </li>
      <li><span class="li-required">system_networkvisibility</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ngfwsettings</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">system_np6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_np6_fpanomaly</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_np6_hpe</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_np6xlite</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_np6xlite_fpanomaly</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_np6xlite_hpe</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_npupost</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_npupost_portnpumap</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_npusetting_prp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_npuvlink</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ntp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ntp_ntpserver</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_passwordpolicy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_passwordpolicyguestadmin</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_pcpserver</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_pcpserver_pools</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_physicalswitch</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_pppoeinterface</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_proberesponse</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_proxyarp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ptp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ptp_serverinterface</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_admin</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_alertmail</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_auth</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_automation</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_custommessage</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_devicedetectionportal</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_fortiguardwf</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_ftp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_http</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_icap</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_mail</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_mm1</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_mm3</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_mm4</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_mm7</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_mms</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_nacquar</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_nntp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_spam</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_sslvpn</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_trafficquota</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_utm</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_replacemsg_webproxy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_saml</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_saml_serviceproviders</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_saml_serviceproviders_assertionattributes</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_sdnvpn</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">system_sdwan</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_sdwan_duplication</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_sdwan_healthcheck</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_sdwan_healthcheck_sla</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_sdwan_healthcheckfortiguard</span> - available versions:
          <span class="li-normal">v7.6.0->latest</span>
      </li>
      <li><span class="li-required">system_sdwan_healthcheckfortiguard_sla</span> - available versions:
          <span class="li-normal">v7.6.0->latest</span>
      </li>
      <li><span class="li-required">system_sdwan_members</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_sdwan_neighbor</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_sdwan_service</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_sdwan_service_sla</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_sdwan_zone</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_securityrating_controls</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">system_securityrating_settings</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">system_sessionhelper</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_sessionttl</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_sessionttl_port</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_settings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_sflow</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_sflow_collectors</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_sittunnel</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_smcntp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_smcntp_ntpserver</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_snmp_community</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_snmp_community_hosts</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_snmp_community_hosts6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_snmp_mibview</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_snmp_rmonstat</span> - available versions:
          <span class="li-normal">v7.6.0->latest</span>
      </li>
      <li><span class="li-required">system_snmp_sysinfo</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_snmp_user</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_speedtestschedule</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_speedtestserver</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_speedtestserver_host</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_speedtestsetting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_splitportmode</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_sshconfig</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ssoadmin</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ssoforticloudadmin</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_ssofortigatecloudadmin</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_standalonecluster</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_standalonecluster_clusterpeer</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_standalonecluster_clusterpeer_sessionsyncfilter</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_standalonecluster_clusterpeer_sessionsyncfilter_customservice</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_standalonecluster_monitorprefix</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">system_storage</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_stp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_switchinterface</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_timezone</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_tosbasedpriority</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_vdom</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_vdomdns</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_vdomexception</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_vdomlink</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_vdomnetflow</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_vdomnetflow_collectors</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_vdomproperty</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_vdomradiusserver</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_vdomsflow</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_vdomsflow_collectors</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_vinalarm</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_virtualswitch</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_virtualswitch_port</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_virtualwanlink</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_virtualwanlink_healthcheck</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_virtualwanlink_healthcheck_sla</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_virtualwanlink_members</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_virtualwanlink_neighbor</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_virtualwanlink_service</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_virtualwanlink_service_sla</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_vneinterface</span> - available versions:
          <span class="li-normal">v7.6.0->latest</span>
      </li>
      <li><span class="li-required">system_vnetunnel</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_vpce</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_vxlan</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_wccp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_wireless_apstatus</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_wireless_settings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_zone</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">system_zone_tagging</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">user_nacpolicy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">user_quarantine</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">user_quarantine_targets</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">user_quarantine_targets_macs</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">user_scim</span> - available versions:
          <span class="li-normal">v7.6.0->latest</span>
      </li>
      <li><span class="li-required">user_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">user_setting_authports</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">videofilter_youtubekey</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>
      </li>
      <li><span class="li-required">vpn_certificate_crl</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_certificate_local</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_certificate_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_certificate_setting_crlverification</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ipsec_concentrator</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ipsec_forticlient</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ipsec_manualkey</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ipsec_manualkeyinterface</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ipsec_phase1</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ipsec_phase1_ipv4excluderange</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ipsec_phase1_ipv6excluderange</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ipsec_phase1interface</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ipsec_phase1interface_ipv4excluderange</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ipsec_phase1interface_ipv6excluderange</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ipsec_phase2</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ipsec_phase2interface</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_kmipserver</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_kmipserver_serverlist</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_l2tp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ocvpn</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ocvpn_forticlientaccess</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ocvpn_forticlientaccess_authgroups</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ocvpn_overlays</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ocvpn_overlays_subnets</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_pptp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_qkd</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ssl_client</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpn_ssl_settings</span> - available versions:
          <span class="li-normal">v6.2.6->v6.2.13</span>,
          <span class="li-normal">v6.4.2->latest</span>
      </li>
      <li><span class="li-required">vpn_ssl_settings_authenticationrule</span> - available versions:
          <span class="li-normal">v6.2.6->v6.2.13</span>,
          <span class="li-normal">v6.4.2->latest</span>
      </li>
      <li><span class="li-required">vpnsslweb_userbookmark</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpnsslweb_userbookmark_bookmarks</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpnsslweb_userbookmark_bookmarks_formdata</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpnsslweb_usergroupbookmark</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpnsslweb_usergroupbookmark_bookmarks</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">vpnsslweb_usergroupbookmark_bookmarks_formdata</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wanopt_cacheservice</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wanopt_cacheservice_dstpeer</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wanopt_cacheservice_srcpeer</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wanopt_contentdeliverynetworkrule</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wanopt_contentdeliverynetworkrule_rules</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wanopt_contentdeliverynetworkrule_rules_contentid</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wanopt_contentdeliverynetworkrule_rules_matchentries</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wanopt_contentdeliverynetworkrule_rules_skipentries</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wanopt_remotestorage</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wanopt_settings</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wanopt_webcache</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">webfilter_fortiguard</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">webfilter_ftgdlocalrisk</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">webfilter_ftgdrisklevel</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">webfilter_ipsurlfiltercachesetting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">webfilter_ipsurlfiltersetting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">webfilter_ipsurlfiltersetting6</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">webfilter_override</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">webfilter_searchengine</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">webproxy_debugurl</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">webproxy_explicit</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">webproxy_explicit_pacpolicy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">webproxy_fastfallback</span> - available versions:
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">webproxy_global</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">webproxy_urlmatch</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_accesscontrollist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_accesscontrollist_layer3ipv4rules</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_accesscontrollist_layer3ipv6rules</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_apcfgprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_apcfgprofile_commandlist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_apstatus</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_arrpprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_bleprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_bonjourprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_bonjourprofile_policylist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_global</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_anqp3gppcellular</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_anqp3gppcellular_mccmnclist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_anqpipaddresstype</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_anqpnairealm</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_anqpnairealm_nailist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_anqpnairealm_nailist_eapmethod</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_anqpnairealm_nailist_eapmethod_authparam</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_anqpnetworkauthtype</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_anqproamingconsortium</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_anqproamingconsortium_oilist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_anqpvenuename</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_anqpvenuename_valuelist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_anqpvenueurl</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_anqpvenueurl_valuelist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_h2qpadviceofcharge</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_h2qpadviceofcharge_aoclist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_h2qpadviceofcharge_aoclist_planinfo</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_h2qpconncapability</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_h2qpoperatorname</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_h2qpoperatorname_valuelist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_h2qposuprovider</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_h2qposuprovider_friendlyname</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_h2qposuprovider_servicedescription</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_h2qposuprovidernai</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_h2qposuprovidernai_nailist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_h2qptermsandconditions</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_h2qpwanmetric</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_hsprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_icon</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_icon_iconlist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_qosmap</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_qosmap_dscpexcept</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_hotspot20_qosmap_dscprange</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_intercontroller</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_intercontroller_intercontrollerpeer</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_log</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_mpskprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_mpskprofile_mpskgroup</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_mpskprofile_mpskgroup_mpskkey</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_nacprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_qosprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_region</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_setting</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_setting_offendingssid</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_snmp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_snmp_community</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_snmp_community_hosts</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_snmp_user</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_ssidpolicy</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_syslogprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_timers</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_utmprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_vap</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_vap_dynamicmapping</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_vap_macfilterlist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_vap_mpskkey</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_vap_portalmessageoverrides</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_vap_vlanname</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_vap_vlanpool</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_vapgroup</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wagprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_widsprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtp</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtp_lan</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtp_radio1</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtp_radio2</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtp_radio3</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtp_radio4</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtp_splittunnelingacl</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtpgroup</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtpprofile</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtpprofile_denymaclist</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtpprofile_eslsesdongle</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtpprofile_lan</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtpprofile_lbs</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtpprofile_platform</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtpprofile_radio1</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtpprofile_radio2</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtpprofile_radio3</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtpprofile_radio4</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">wireless_wtpprofile_splittunnelingacl</span> - available versions:
          <span class="li-normal">v7.2.6->v7.2.9</span>,
          <span class="li-normal">v7.4.3->latest</span>
      </li>
      <li><span class="li-required">ztna_reverseconnector</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">ztna_trafficforwardproxy</span> - available versions:
          <span class="li-normal">v7.6.0->latest</span>
      </li>
      <li><span class="li-required">ztna_trafficforwardproxy_quic</span> - available versions:
          <span class="li-normal">v7.6.0->latest</span>
      </li>
      <li><span class="li-required">ztna_trafficforwardproxy_sslciphersuites</span> - available versions:
          <span class="li-normal">v7.6.0->latest</span>
      </li>
      <li><span class="li-required">ztna_trafficforwardproxy_sslserverciphersuites</span> - available versions:
          <span class="li-normal">v7.6.0->latest</span>
      </li>
      <li><span class="li-required">ztna_trafficforwardproxyreverseservice</span> - available versions:
          <span class="li-normal">v7.6.0->latest</span>
      </li>
      <li><span class="li-required">ztna_trafficforwardproxyreverseservice_remoteservers</span> - available versions:
          <span class="li-normal">v7.6.0->latest</span>
      </li>
      <li><span class="li-required">ztna_webportal</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">ztna_webportalbookmark</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">ztna_webportalbookmark_bookmarks</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">ztna_webproxy</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">ztna_webproxy_apigateway</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">ztna_webproxy_apigateway6</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">ztna_webproxy_apigateway6_quic</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">ztna_webproxy_apigateway6_realservers</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">ztna_webproxy_apigateway6_sslciphersuites</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">ztna_webproxy_apigateway_quic</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">ztna_webproxy_apigateway_realservers</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
      <li><span class="li-required">ztna_webproxy_apigateway_sslciphersuites</span> - available versions:
          <span class="li-normal">v7.6.2->latest</span>
      </li>
  </ul>
  </div>
  </section>
  <li><span class="li-head">fields</span> - Limit the output by returning only the attributes specified in the string array.  <span class="li-normal">type: list</span> <span class="li-required">required: false</span></li>
  <li><span class="li-head">filter</span> - Filter the result according to a set of criteria. <span class="li-normal">type: list</span> <span class="li-required">required: false</span></li>
  <li><span class="li-head">option</span> - Set fetch option for the request. If no option is specified, by default the attributes of the objects will be returned. See more details in FNDN API documents. <span class="li-normal">type: str</span> <span class="li-required">required: false</span></li>
  <li><span class="li-head">sortings</span> - Sorting rules list: items are returned in ascending(1) or descending(-1) order of fields in the list. <span class="li-normal">type: list of dict</span> <span class="li-required">required: false</span></li>
  <li><span class="li-head">params</span> - the parameter for each selector <span class="li-normal">type: dict</span> <span class="li-required">choices:</span></li>
  <li style="list-style: none;"><section class="accordion">
  <input type="checkbox" name="collapse" id="handle3">
  <h2 class="handle">
    <label for="handle3"><u>More details about parameter: <b>params</b>...</u></label>
  </h2>
  <div class="content">
     
  <ul class="ul-self">
        <li><span class="li-normal">params for alertemail_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for antivirus_exemptlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">exempt-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for antivirus_heuristic:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for antivirus_quarantine:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for antivirus_settings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for application_name:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for application_rulesettings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for automation_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for aws_vpce:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vpce</span></li>
        </ul>
        <li><span class="li-normal">params for azure_vwaningresspublicips:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vwan-ingress-public-IPs</span></li>
        </ul>
        <li><span class="li-normal">params for azure_vwanslb:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for azure_vwanslb_permanentsecurityrules:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for azure_vwanslb_permanentsecurityrules_rules:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">rules</span></li>
        </ul>
        <li><span class="li-normal">params for azure_vwanslb_temporarysecurityrules:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for azure_vwanslb_temporarysecurityrules_rules:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">rules</span></li>
        </ul>
        <li><span class="li-normal">params for casb_attributematch:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">attribute-match</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for casb_attributematch_attribute:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">attribute</span></li>
            <li><span class="li-normal">attribute-match</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for certificate_remote:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">remote</span></li>
        </ul>
        <li><span class="li-normal">params for dlp_exactdatamatch:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">exact-data-match</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for dlp_exactdatamatch_columns:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">columns</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">exact-data-match</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for dlp_fpdocsource:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">fp-doc-source</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for dlp_settings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for dpdk_cpus:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for dpdk_global:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for emailfilter_fortiguard:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for endpointcontrol_fctemsoverride:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">fctems-override</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for endpointcontrol_settings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for ethernetoam_cfm:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">cfm</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for ethernetoam_cfm_service:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">cfm</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">service</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for extendercontroller_extender:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">extender</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for extendercontroller_extender_controllerreport:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">extender</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for extendercontroller_extender_modem1:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">extender</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for extendercontroller_extender_modem1_autoswitch:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">extender</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for extendercontroller_extender_modem2:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">extender</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for extendercontroller_extender_modem2_autoswitch:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">extender</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for extendercontroller_extender_wanextension:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">extender</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for extensioncontroller_extender:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">extender</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for extensioncontroller_extender_wanextension:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">extender</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for extensioncontroller_extendervap:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">extender-vap</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for extensioncontroller_fortigate:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">fortigate</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for extensioncontroller_fortigateprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">fortigate-profile</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for extensioncontroller_fortigateprofile_lanextension:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">fortigate-profile</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_accessproxysshclientcert:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">access-proxy-ssh-client-cert</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_accessproxysshclientcert_certextension:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">access-proxy-ssh-client-cert</span></li>
            <li><span class="li-normal">cert-extension</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_authportal:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_dnstranslation:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">dnstranslation</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_global:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_internetserviceappend:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_internetservicedefinition:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">internet-service-definition</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_internetservicedefinition_entry:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">entry</span></li>
            <li><span class="li-normal">internet-service-definition</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_internetservicedefinition_entry_portrange:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">entry</span></li>
            <li><span class="li-normal">internet-service-definition</span></li>
            <li><span class="li-normal">port-range</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_internetserviceextension:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">internet-service-extension</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_internetserviceextension_disableentry:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">disable-entry</span></li>
            <li><span class="li-normal">internet-service-extension</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_internetserviceextension_disableentry_ip6range:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">disable-entry</span></li>
            <li><span class="li-normal">internet-service-extension</span></li>
            <li><span class="li-normal">ip6-range</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_internetserviceextension_disableentry_iprange:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">disable-entry</span></li>
            <li><span class="li-normal">internet-service-extension</span></li>
            <li><span class="li-normal">ip-range</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_internetserviceextension_disableentry_portrange:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">disable-entry</span></li>
            <li><span class="li-normal">internet-service-extension</span></li>
            <li><span class="li-normal">port-range</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_internetserviceextension_entry:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">entry</span></li>
            <li><span class="li-normal">internet-service-extension</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_internetserviceextension_entry_portrange:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">entry</span></li>
            <li><span class="li-normal">internet-service-extension</span></li>
            <li><span class="li-normal">port-range</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_ipmacbinding_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_ipmacbinding_table:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">table</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_iptranslation:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ip-translation</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_ipv6ehfilter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_ondemandsniffer:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">on-demand-sniffer</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_pfcp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">pfcp</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_policy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_sniffer:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">sniffer</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_sniffer_anomaly:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">anomaly</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">sniffer</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_ssh_hostkey:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">host-key</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_ssh_localkey:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">local-key</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_ssh_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_ssl_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_sslserver:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ssl-server</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for firewall_ttlpolicy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ttl-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for ftpproxy_explicit:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for gtp_apnshaper:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">apn-shaper</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for gtp_ieallowlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ie-allow-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for gtp_ieallowlist_entries:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">entries</span></li>
            <li><span class="li-normal">ie-allow-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for gtp_rattimeoutprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">rat-timeout-profile</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for icap_profile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">profile</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for icap_server:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">server</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for icap_servergroup:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">server-group</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for icap_servergroup_serverlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">server-group</span></li>
            <li><span class="li-normal">server-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for ips_decoder:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for ips_decoder_parameter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for ips_global:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for ips_rule:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for ips_rulesettings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for ips_settings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for ips_tlsactiveprobe:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for loadbalance_flowrule:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">flow-rule</span></li>
        </ul>
        <li><span class="li-normal">params for loadbalance_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for loadbalance_setting_workers:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">workers</span></li>
        </ul>
        <li><span class="li-normal">params for loadbalance_workergroup:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">worker-group</span></li>
        </ul>
        <li><span class="li-normal">params for log_azuresecuritycenter2_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_azuresecuritycenter2_filter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
        </ul>
        <li><span class="li-normal">params for log_azuresecuritycenter2_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_azuresecuritycenter2_setting_customfieldname:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">custom-field-name</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_azuresecuritycenter_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_azuresecuritycenter_filter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
        </ul>
        <li><span class="li-normal">params for log_azuresecuritycenter_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_azuresecuritycenter_setting_customfieldname:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">custom-field-name</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_disk_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_disk_filter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_disk_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_eventfilter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer2_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer2_filter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer2_overridefilter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer2_overridefilter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer2_overridesetting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer2_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer3_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer3_filter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer3_overridefilter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer3_overridefilter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer3_overridesetting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer3_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer_filter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer_overridefilter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer_overridefilter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer_overridesetting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzer_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzercloud_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzercloud_filter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzercloud_overridefilter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzercloud_overridefilter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzercloud_overridesetting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortianalyzercloud_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortiguard_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortiguard_filter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortiguard_overridefilter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortiguard_overridefilter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortiguard_overridesetting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_fortiguard_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_guidisplay:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_memory_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_memory_filter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_memory_globalsetting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_memory_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_nulldevice_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_nulldevice_filter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_nulldevice_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_slbc_globalsetting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd2_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd2_filter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd2_overridefilter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd2_overridefilter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd2_overridesetting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd2_overridesetting_customfieldname:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">custom-field-name</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd2_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd2_setting_customfieldname:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">custom-field-name</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd3_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd3_filter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd3_overridefilter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd3_overridefilter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd3_overridesetting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd3_overridesetting_customfieldname:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">custom-field-name</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd3_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd3_setting_customfieldname:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">custom-field-name</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd4_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd4_filter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd4_overridefilter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd4_overridefilter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd4_overridesetting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd4_overridesetting_customfieldname:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">custom-field-name</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd4_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd4_setting_customfieldname:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">custom-field-name</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd_filter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd_overridefilter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd_overridefilter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd_overridesetting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd_overridesetting_customfieldname:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">custom-field-name</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_syslogd_setting_customfieldname:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">custom-field-name</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_tacacsaccounting2_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_tacacsaccounting2_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_tacacsaccounting3_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_tacacsaccounting3_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_tacacsaccounting_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_tacacsaccounting_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for log_webtrends_filter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for log_webtrends_filter_freestyle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">free-style</span></li>
        </ul>
        <li><span class="li-normal">params for log_webtrends_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for monitoring_np6ipsecengine:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for monitoring_npuhpe:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for notification:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for nsx_profile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">profile</span></li>
        </ul>
        <li><span class="li-normal">params for nsxt_servicechain:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">service-chain</span></li>
        </ul>
        <li><span class="li-normal">params for nsxt_servicechain_serviceindex:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">service-chain</span></li>
            <li><span class="li-normal">service-index</span></li>
        </ul>
        <li><span class="li-normal">params for nsxt_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for pfcp_messagefilter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">message-filter</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_chart:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">chart</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_chart_categoryseries:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">chart</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_chart_column:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">chart</span></li>
            <li><span class="li-normal">column</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_chart_column_mapping:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">chart</span></li>
            <li><span class="li-normal">column</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">mapping</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_chart_drilldowncharts:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">chart</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">drill-down-charts</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_chart_valueseries:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">chart</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_chart_xseries:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">chart</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_chart_yseries:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">chart</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_dataset:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">dataset</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_dataset_field:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">dataset</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">field</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_dataset_parameters:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">dataset</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">parameters</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_layout:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">layout</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_layout_bodyitem:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">body-item</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">layout</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_layout_bodyitem_list:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">body-item</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">layout</span></li>
            <li><span class="li-normal">list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_layout_bodyitem_parameters:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">body-item</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">layout</span></li>
            <li><span class="li-normal">parameters</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_layout_page:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">layout</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_layout_page_footer:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">layout</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_layout_page_footer_footeritem:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">footer-item</span></li>
            <li><span class="li-normal">layout</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_layout_page_header:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">layout</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_layout_page_header_headeritem:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">header-item</span></li>
            <li><span class="li-normal">layout</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_style:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">style</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for report_theme:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">theme</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_authpath:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">auth-path</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bfd:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bfd6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bfd6_multihoptemplate:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">multihop-template</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bfd6_neighbor:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">neighbor</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bfd_multihoptemplate:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">multihop-template</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bfd_neighbor:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">neighbor</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_admindistance:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">admin-distance</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_aggregateaddress:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">aggregate-address</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_aggregateaddress6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">aggregate-address6</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_neighbor:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">neighbor</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_neighbor_conditionaladvertise:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">conditional-advertise</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">neighbor</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_neighbor_conditionaladvertise6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">conditional-advertise6</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">neighbor</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_neighborgroup:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">neighbor-group</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_neighborrange:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">neighbor-range</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_neighborrange6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">neighbor-range6</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_network:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">network</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_network6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">network6</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_redistribute:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_redistribute6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_vrf:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">vrf</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_vrf6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">vrf6</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_vrf6_leaktarget:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">leak-target</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">vrf6</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_vrf_leaktarget:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">leak-target</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">vrf</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_vrfleak:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">vrf-leak</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_vrfleak6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">vrf-leak6</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_vrfleak6_target:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">target</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">vrf-leak6</span></li>
        </ul>
        <li><span class="li-normal">params for router_bgp_vrfleak_target:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">target</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">vrf-leak</span></li>
        </ul>
        <li><span class="li-normal">params for router_extcommunitylist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">extcommunity-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_extcommunitylist_rule:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">extcommunity-list</span></li>
            <li><span class="li-normal">rule</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_isis:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_isis_isisinterface:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">isis-interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_isis_isisnet:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">isis-net</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_isis_redistribute:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_isis_redistribute6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_isis_summaryaddress:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">summary-address</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_isis_summaryaddress6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">summary-address6</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_keychain:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">key-chain</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_keychain_key:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">key</span></li>
            <li><span class="li-normal">key-chain</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_multicast:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_multicast6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_multicast6_interface:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_multicast6_pimsmglobal:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_multicast6_pimsmglobal_rpaddress:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">rp-address</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_multicast_interface:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_multicast_interface_igmp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_multicast_interface_joingroup:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">join-group</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_multicast_pimsmglobal:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_multicast_pimsmglobal_rpaddress:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">rp-address</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_multicast_pimsmglobalvrf:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">pim-sm-global-vrf</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_multicast_pimsmglobalvrf_rpaddress:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">pim-sm-global-vrf</span></li>
            <li><span class="li-normal">rp-address</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_multicastflow:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">multicast-flow</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_multicastflow_flows:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">flows</span></li>
            <li><span class="li-normal">multicast-flow</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf6_area:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">area</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf6_area_ipseckeys:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">area</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ipsec-keys</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf6_area_range:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">area</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">range</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf6_area_virtuallink:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">area</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">virtual-link</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf6_area_virtuallink_ipseckeys:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">area</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ipsec-keys</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">virtual-link</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf6_ospf6interface:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ospf6-interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf6_ospf6interface_ipseckeys:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ipsec-keys</span></li>
            <li><span class="li-normal">ospf6-interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf6_ospf6interface_neighbor:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">neighbor</span></li>
            <li><span class="li-normal">ospf6-interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf6_redistribute:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf6_summaryaddress:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">summary-address</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf_area:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">area</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf_area_filterlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">area</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">filter-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf_area_range:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">area</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">range</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf_area_virtuallink:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">area</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">virtual-link</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf_area_virtuallink_md5keys:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">area</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">md5-keys</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">virtual-link</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf_distributelist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">distribute-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf_neighbor:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">neighbor</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf_network:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">network</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf_ospfinterface:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ospf-interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf_ospfinterface_md5keys:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">md5-keys</span></li>
            <li><span class="li-normal">ospf-interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf_redistribute:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ospf_summaryaddress:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">summary-address</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_policy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_policy6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">policy6</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_rip:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_rip_distance:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">distance</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_rip_distributelist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">distribute-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_rip_interface:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_rip_neighbor:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">neighbor</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_rip_network:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">network</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_rip_offsetlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">offset-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_rip_redistribute:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ripng:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ripng_aggregateaddress:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">aggregate-address</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ripng_distance:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">distance</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ripng_distributelist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">distribute-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ripng_interface:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ripng_neighbor:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">neighbor</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ripng_network:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">network</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ripng_offsetlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">offset-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_ripng_redistribute:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_routemap:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">route-map</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_static:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">static</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for router_static6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">static6</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for rule_fmwp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for rule_otdt:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for rule_otvp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_8021xsettings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_acl_group:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">group</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_acl_ingress:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ingress</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_acl_ingress_action:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ingress</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_acl_ingress_classifier:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ingress</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_autoconfig_custom:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">custom</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_autoconfig_custom_switchbinding:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">custom</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">switch-binding</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_autoconfig_default:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_autoconfig_policy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_customcommand:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">custom-command</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_dsl_policy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_dynamicportpolicy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">dynamic-port-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_dynamicportpolicy_policy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">dynamic-port-policy</span></li>
            <li><span class="li-normal">policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_flowtracking:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_flowtracking_aggregates:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">aggregates</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_flowtracking_collectors:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">collectors</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_fortilinksettings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">fortilink-settings</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_fortilinksettings_nacports:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">fortilink-settings</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_global:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_igmpsnooping:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_initialconfig_template:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">template</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_initialconfig_vlans:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_lldpprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">lldp-profile</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_lldpprofile_customtlvs:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">custom-tlvs</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">lldp-profile</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_lldpprofile_medlocationservice:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">lldp-profile</span></li>
            <li><span class="li-normal">med-location-service</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_lldpprofile_mednetworkpolicy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">lldp-profile</span></li>
            <li><span class="li-normal">med-network-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_lldpsettings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_location:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">location</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_location_addresscivic:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">location</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_location_coordinates:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">location</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_location_elinnumber:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">location</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_macpolicy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">mac-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_8021xsettings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_customcommand:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">custom-command</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_dhcpsnoopingstaticclient:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">dhcp-snooping-static-client</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_igmpsnooping:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_igmpsnooping_vlans:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">vlans</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_ipsourceguard:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ip-source-guard</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_ipsourceguard_bindingentry:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">binding-entry</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ip-source-guard</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_mirror:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">mirror</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_ports:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">ports</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_ports_dhcpsnoopoption82override:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">dhcp-snoop-option82-override</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">ports</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_remotelog:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">remote-log</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_routeoffloadrouter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">route-offload-router</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_snmpcommunity:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">snmp-community</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_snmpcommunity_hosts:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">hosts</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">snmp-community</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_snmpsysinfo:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_snmptrapthreshold:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_snmpuser:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">snmp-user</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_staticmac:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">static-mac</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_stormcontrol:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_stpinstance:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">stp-instance</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_stpsettings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_switchlog:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_managedswitch_vlan:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">managed-switch</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">vlan</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_nacdevice:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">nac-device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_nacsettings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">nac-settings</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_networkmonitorsettings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_portpolicy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">port-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_ptp_interfacepolicy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_ptp_policy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_ptp_profile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">profile</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_ptp_settings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_qos_dot1pmap:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">dot1p-map</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_qos_ipdscpmap:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ip-dscp-map</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_qos_ipdscpmap_map:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ip-dscp-map</span></li>
            <li><span class="li-normal">map</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_qos_qospolicy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">qos-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_qos_queuepolicy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">queue-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_qos_queuepolicy_cosqueue:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">cos-queue</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">queue-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_remotelog:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">remote-log</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_securitypolicy_8021x:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">802-1X</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_securitypolicy_localaccess:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">local-access</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_sflow:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_snmpcommunity:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">snmp-community</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_snmpcommunity_hosts:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">hosts</span></li>
            <li><span class="li-normal">snmp-community</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_snmpsysinfo:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_snmptrapthreshold:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_snmpuser:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">snmp-user</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_stormcontrol:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_stormcontrolpolicy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">storm-control-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_stpinstance:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">stp-instance</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_stpsettings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_switchgroup:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">switch-group</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_switchinterfacetag:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">switch-interface-tag</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_switchlog:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_switchprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">switch-profile</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_system:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_trafficpolicy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">traffic-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_trafficsniffer:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_trafficsniffer_targetip:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">target-ip</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_trafficsniffer_targetmac:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">target-mac</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_trafficsniffer_targetport:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">target-port</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_virtualportpool:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">virtual-port-pool</span></li>
        </ul>
        <li><span class="li-normal">params for switchcontroller_vlanpolicy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">vlan-policy</span></li>
        </ul>
        <li><span class="li-normal">params for system_3gmodem_custom:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">custom</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_5gmodem:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_5gmodem_dataplan:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">data-plan</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_5gmodem_modem1:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_5gmodem_modem1_simswitch:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_5gmodem_modem2:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_accprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">accprofile</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_accprofile_fwgrppermission:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">accprofile</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_accprofile_loggrppermission:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">accprofile</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_accprofile_netgrppermission:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">accprofile</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_accprofile_sysgrppermission:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">accprofile</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_accprofile_utmgrppermission:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">accprofile</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_acme:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_acme_accounts:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">accounts</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_admin:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">admin</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_affinityinterrupt:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">affinity-interrupt</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_affinitypacketredistribution:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">affinity-packet-redistribution</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_alias:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">alias</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_apiuser:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">api-user</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_apiuser_trusthost:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">api-user</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">trusthost</span></li>
        </ul>
        <li><span class="li-normal">params for system_arptable:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">arp-table</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_autoinstall:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_automationaction:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">automation-action</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_automationaction_httpheaders:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">automation-action</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">http-headers</span></li>
        </ul>
        <li><span class="li-normal">params for system_automationcondition:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">automation-condition</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_automationdestination:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">automation-destination</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_automationstitch:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">automation-stitch</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_automationstitch_actions:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">actions</span></li>
            <li><span class="li-normal">automation-stitch</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_automationtrigger:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">automation-trigger</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_automationtrigger_fields:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">automation-trigger</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">fields</span></li>
        </ul>
        <li><span class="li-normal">params for system_autoscale:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_autoscript:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">auto-script</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_autoupdate_pushupdate:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_autoupdate_schedule:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_autoupdate_tunneling:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_bypass:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_centralmanagement:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_centralmanagement_serverlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">server-list</span></li>
        </ul>
        <li><span class="li-normal">params for system_clustersync:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">cluster-sync</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_clustersync_sessionsyncfilter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">cluster-sync</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_clustersync_sessionsyncfilter_customservice:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">cluster-sync</span></li>
            <li><span class="li-normal">custom-service</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_console:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_consoleserver:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_consoleserver_entries:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">entries</span></li>
        </ul>
        <li><span class="li-normal">params for system_csf:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_csf_fabricconnector:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">fabric-connector</span></li>
        </ul>
        <li><span class="li-normal">params for system_csf_fabricdevice:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">fabric-device</span></li>
        </ul>
        <li><span class="li-normal">params for system_csf_trustedlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">trusted-list</span></li>
        </ul>
        <li><span class="li-normal">params for system_ddns:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">ddns</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_dedicatedmgmt:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_deviceupgrade:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">device-upgrade</span></li>
        </ul>
        <li><span class="li-normal">params for system_deviceupgrade_knownhamembers:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">device-upgrade</span></li>
            <li><span class="li-normal">known-ha-members</span></li>
        </ul>
        <li><span class="li-normal">params for system_dhcp6_server:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">server</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_dhcp6_server_iprange:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ip-range</span></li>
            <li><span class="li-normal">server</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_dhcp6_server_options:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">options</span></li>
            <li><span class="li-normal">server</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_dhcp6_server_prefixrange:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">prefix-range</span></li>
            <li><span class="li-normal">server</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_digitalio:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_dnp3proxy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_dns:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_dns64:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_dnsdatabase:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">dns-database</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_dnsdatabase_dnsentry:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">dns-database</span></li>
            <li><span class="li-normal">dns-entry</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_dnsserver:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">dns-server</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_dscpbasedpriority:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">dscp-based-priority</span></li>
        </ul>
        <li><span class="li-normal">params for system_elbc:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_emailserver:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_evpn:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">evpn</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_fabricvpn:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_fabricvpn_advertisedsubnets:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">advertised-subnets</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_fabricvpn_overlays:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">overlays</span></li>
        </ul>
        <li><span class="li-normal">params for system_federatedupgrade:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_federatedupgrade_knownhamembers:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">known-ha-members</span></li>
        </ul>
        <li><span class="li-normal">params for system_federatedupgrade_nodelist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">node-list</span></li>
        </ul>
        <li><span class="li-normal">params for system_fipscc:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_fortiai:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_fortindr:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_fortisandbox:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_fssopolling:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ftmpush:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_geneve:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">geneve</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_gigk:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_global:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_gretunnel:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">gre-tunnel</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_ha:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ha_frupsettings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ha_hamgmtinterfaces:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ha-mgmt-interfaces</span></li>
        </ul>
        <li><span class="li-normal">params for system_ha_secondaryvcluster:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ha_unicastpeers:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">unicast-peers</span></li>
        </ul>
        <li><span class="li-normal">params for system_ha_vcluster:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vcluster</span></li>
        </ul>
        <li><span class="li-normal">params for system_hamonitor:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_healthcheckfortiguard:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">health-check-fortiguard</span></li>
        </ul>
        <li><span class="li-normal">params for system_icond:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup1:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup14:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup15:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup16:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup17:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup18:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup19:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup2:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup20:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup21:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup27:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup28:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup29:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup30:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup31:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup32:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ike_dhgroup5:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_clientoptions:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">client-options</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_dhcpsnoopingserverlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">dhcp-snooping-server-list</span></li>
            <li><span class="li-normal">interface</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_egressqueues:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_ipv6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_ipv6_clientoptions:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">client-options</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_ipv6_dhcp6iapdlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">dhcp6-iapd-list</span></li>
            <li><span class="li-normal">interface</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_ipv6_ip6delegatedprefixlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">ip6-delegated-prefix-list</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_ipv6_ip6dnssllist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">ip6-dnssl-list</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_ipv6_ip6extraaddr:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">ip6-extra-addr</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_ipv6_ip6prefixlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">ip6-prefix-list</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_ipv6_ip6rdnsslist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">ip6-rdnss-list</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_ipv6_ip6routelist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">ip6-route-list</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_ipv6_vrrp6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">vrrp6</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_l2tpclientsettings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_mirroringfilter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_secondaryip:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">secondaryip</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_tagging:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">tagging</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_vrrp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">vrrp</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_vrrp_proxyarp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">proxy-arp</span></li>
            <li><span class="li-normal">vrrp</span></li>
        </ul>
        <li><span class="li-normal">params for system_interface_wifinetworks:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">interface</span></li>
            <li><span class="li-normal">wifi-networks</span></li>
        </ul>
        <li><span class="li-normal">params for system_ipam:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ipam_pools:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">pools</span></li>
        </ul>
        <li><span class="li-normal">params for system_ipam_pools_exclude:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">exclude</span></li>
            <li><span class="li-normal">pools</span></li>
        </ul>
        <li><span class="li-normal">params for system_ipam_rules:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">rules</span></li>
        </ul>
        <li><span class="li-normal">params for system_ipiptunnel:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ipip-tunnel</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_ips:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_ipsecaggregate:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ipsec-aggregate</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_ipsurlfilterdns:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ips-urlfilter-dns</span></li>
        </ul>
        <li><span class="li-normal">params for system_ipsurlfilterdns6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ips-urlfilter-dns6</span></li>
        </ul>
        <li><span class="li-normal">params for system_ipv6neighborcache:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ipv6-neighbor-cache</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_ipv6tunnel:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ipv6-tunnel</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_iscsi:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">iscsi</span></li>
        </ul>
        <li><span class="li-normal">params for system_isfqueueprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">isf-queue-profile</span></li>
        </ul>
        <li><span class="li-normal">params for system_linkmonitor:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">link-monitor</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_linkmonitor_serverlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">link-monitor</span></li>
            <li><span class="li-normal">server-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_lldp_networkpolicy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">network-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_lldp_networkpolicy_guest:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">network-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_lldp_networkpolicy_guestvoicesignaling:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">network-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_lldp_networkpolicy_softphone:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">network-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_lldp_networkpolicy_streamingvideo:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">network-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_lldp_networkpolicy_videoconferencing:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">network-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_lldp_networkpolicy_videosignaling:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">network-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_lldp_networkpolicy_voice:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">network-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_lldp_networkpolicy_voicesignaling:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">network-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_ltemodem:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ltemodem_dataplan:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">data-plan</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ltemodem_simswitch:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_macaddresstable:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">mac-address-table</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_memmgr:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_mobiletunnel:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">mobile-tunnel</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_mobiletunnel_network:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">mobile-tunnel</span></li>
            <li><span class="li-normal">network</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_modem:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_nat64:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_nat64_secondaryprefix:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">secondary-prefix</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_ndproxy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_netflow:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_netflow_collectors:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">collectors</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_netflow_exclusionfilters:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">exclusion-filters</span></li>
        </ul>
        <li><span class="li-normal">params for system_networkvisibility:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_ngfwsettings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_np6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">np6</span></li>
        </ul>
        <li><span class="li-normal">params for system_np6_fpanomaly:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">np6</span></li>
        </ul>
        <li><span class="li-normal">params for system_np6_hpe:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">np6</span></li>
        </ul>
        <li><span class="li-normal">params for system_np6xlite:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">np6xlite</span></li>
        </ul>
        <li><span class="li-normal">params for system_np6xlite_fpanomaly:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">np6xlite</span></li>
        </ul>
        <li><span class="li-normal">params for system_np6xlite_hpe:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">np6xlite</span></li>
        </ul>
        <li><span class="li-normal">params for system_npupost:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_npupost_portnpumap:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">port-npu-map</span></li>
        </ul>
        <li><span class="li-normal">params for system_npusetting_prp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_npuvlink:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">npu-vlink</span></li>
        </ul>
        <li><span class="li-normal">params for system_ntp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ntp_ntpserver:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ntpserver</span></li>
        </ul>
        <li><span class="li-normal">params for system_passwordpolicy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_passwordpolicyguestadmin:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_pcpserver:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_pcpserver_pools:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">pools</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_physicalswitch:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">physical-switch</span></li>
        </ul>
        <li><span class="li-normal">params for system_pppoeinterface:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">pppoe-interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_proberesponse:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_proxyarp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">proxy-arp</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_ptp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ptp_serverinterface:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">server-interface</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_admin:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_alertmail:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_auth:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_automation:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_custommessage:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_devicedetectionportal:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_fortiguardwf:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_ftp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_http:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_icap:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_mail:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_mm1:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_mm3:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_mm4:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_mm7:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_mms:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_nacquar:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_nntp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_spam:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_sslvpn:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_trafficquota:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_utm:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_replacemsg_webproxy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_saml:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_saml_serviceproviders:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">service-providers</span></li>
        </ul>
        <li><span class="li-normal">params for system_saml_serviceproviders_assertionattributes:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">assertion-attributes</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">service-providers</span></li>
        </ul>
        <li><span class="li-normal">params for system_sdnvpn:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">sdn-vpn</span></li>
        </ul>
        <li><span class="li-normal">params for system_sdwan:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_sdwan_duplication:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">duplication</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_sdwan_healthcheck:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">health-check</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_sdwan_healthcheck_sla:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">health-check</span></li>
            <li><span class="li-normal">sla</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_sdwan_healthcheckfortiguard:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">health-check-fortiguard</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_sdwan_healthcheckfortiguard_sla:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">health-check-fortiguard</span></li>
            <li><span class="li-normal">sla</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_sdwan_members:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">members</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_sdwan_neighbor:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">neighbor</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_sdwan_service:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">service</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_sdwan_service_sla:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">service</span></li>
            <li><span class="li-normal">sla</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_sdwan_zone:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">zone</span></li>
        </ul>
        <li><span class="li-normal">params for system_securityrating_controls:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">controls</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_securityrating_settings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_sessionhelper:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">session-helper</span></li>
        </ul>
        <li><span class="li-normal">params for system_sessionttl:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_sessionttl_port:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">port</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_settings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_sflow:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_sflow_collectors:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">collectors</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_sittunnel:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">sit-tunnel</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_smcntp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_smcntp_ntpserver:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ntpserver</span></li>
        </ul>
        <li><span class="li-normal">params for system_snmp_community:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">community</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_snmp_community_hosts:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">community</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">hosts</span></li>
        </ul>
        <li><span class="li-normal">params for system_snmp_community_hosts6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">community</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">hosts6</span></li>
        </ul>
        <li><span class="li-normal">params for system_snmp_mibview:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">mib-view</span></li>
        </ul>
        <li><span class="li-normal">params for system_snmp_rmonstat:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">rmon-stat</span></li>
        </ul>
        <li><span class="li-normal">params for system_snmp_sysinfo:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_snmp_user:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">user</span></li>
        </ul>
        <li><span class="li-normal">params for system_speedtestschedule:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">speed-test-schedule</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_speedtestserver:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">speed-test-server</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_speedtestserver_host:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">host</span></li>
            <li><span class="li-normal">speed-test-server</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_speedtestsetting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_splitportmode:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">split-port-mode</span></li>
        </ul>
        <li><span class="li-normal">params for system_sshconfig:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_ssoadmin:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">sso-admin</span></li>
        </ul>
        <li><span class="li-normal">params for system_ssoforticloudadmin:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">sso-forticloud-admin</span></li>
        </ul>
        <li><span class="li-normal">params for system_ssofortigatecloudadmin:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">sso-fortigate-cloud-admin</span></li>
        </ul>
        <li><span class="li-normal">params for system_standalonecluster:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_standalonecluster_clusterpeer:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">cluster-peer</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_standalonecluster_clusterpeer_sessionsyncfilter:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">cluster-peer</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_standalonecluster_clusterpeer_sessionsyncfilter_customservice:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">cluster-peer</span></li>
            <li><span class="li-normal">custom-service</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_standalonecluster_monitorprefix:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">monitor-prefix</span></li>
        </ul>
        <li><span class="li-normal">params for system_storage:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">storage</span></li>
        </ul>
        <li><span class="li-normal">params for system_stp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_switchinterface:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">switch-interface</span></li>
        </ul>
        <li><span class="li-normal">params for system_timezone:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_tosbasedpriority:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">tos-based-priority</span></li>
        </ul>
        <li><span class="li-normal">params for system_vdom:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_vdomdns:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_vdomexception:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom-exception</span></li>
        </ul>
        <li><span class="li-normal">params for system_vdomlink:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom-link</span></li>
        </ul>
        <li><span class="li-normal">params for system_vdomnetflow:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_vdomnetflow_collectors:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">collectors</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_vdomproperty:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom-property</span></li>
        </ul>
        <li><span class="li-normal">params for system_vdomradiusserver:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom-radius-server</span></li>
        </ul>
        <li><span class="li-normal">params for system_vdomsflow:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_vdomsflow_collectors:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">collectors</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_vinalarm:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_virtualswitch:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">virtual-switch</span></li>
        </ul>
        <li><span class="li-normal">params for system_virtualswitch_port:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">port</span></li>
            <li><span class="li-normal">virtual-switch</span></li>
        </ul>
        <li><span class="li-normal">params for system_virtualwanlink:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_virtualwanlink_healthcheck:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">health-check</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_virtualwanlink_healthcheck_sla:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">health-check</span></li>
            <li><span class="li-normal">sla</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_virtualwanlink_members:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">members</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_virtualwanlink_neighbor:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">neighbor</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_virtualwanlink_service:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">service</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_virtualwanlink_service_sla:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">service</span></li>
            <li><span class="li-normal">sla</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_vneinterface:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">vne-interface</span></li>
        </ul>
        <li><span class="li-normal">params for system_vnetunnel:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for system_vpce:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vpce</span></li>
        </ul>
        <li><span class="li-normal">params for system_vxlan:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">vxlan</span></li>
        </ul>
        <li><span class="li-normal">params for system_wccp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wccp</span></li>
        </ul>
        <li><span class="li-normal">params for system_wireless_apstatus:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">ap-status</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_wireless_settings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for system_zone:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">zone</span></li>
        </ul>
        <li><span class="li-normal">params for system_zone_tagging:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">tagging</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">zone</span></li>
        </ul>
        <li><span class="li-normal">params for user_nacpolicy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">nac-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for user_quarantine:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for user_quarantine_targets:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">targets</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for user_quarantine_targets_macs:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">macs</span></li>
            <li><span class="li-normal">targets</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for user_scim:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">scim</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for user_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for user_setting_authports:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">auth-ports</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for videofilter_youtubekey:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">youtube-key</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_certificate_crl:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">crl</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_certificate_local:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">local</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_certificate_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_certificate_setting_crlverification:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ipsec_concentrator:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">concentrator</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ipsec_forticlient:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">forticlient</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ipsec_manualkey:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">manualkey</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ipsec_manualkeyinterface:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">manualkey-interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ipsec_phase1:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">phase1</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ipsec_phase1_ipv4excluderange:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ipv4-exclude-range</span></li>
            <li><span class="li-normal">phase1</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ipsec_phase1_ipv6excluderange:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ipv6-exclude-range</span></li>
            <li><span class="li-normal">phase1</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ipsec_phase1interface:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">phase1-interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ipsec_phase1interface_ipv4excluderange:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ipv4-exclude-range</span></li>
            <li><span class="li-normal">phase1-interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ipsec_phase1interface_ipv6excluderange:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ipv6-exclude-range</span></li>
            <li><span class="li-normal">phase1-interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ipsec_phase2:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">phase2</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ipsec_phase2interface:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">phase2-interface</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_kmipserver:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">kmip-server</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_kmipserver_serverlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">kmip-server</span></li>
            <li><span class="li-normal">server-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_l2tp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ocvpn:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ocvpn_forticlientaccess:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ocvpn_forticlientaccess_authgroups:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">auth-groups</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ocvpn_overlays:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">overlays</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ocvpn_overlays_subnets:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">overlays</span></li>
            <li><span class="li-normal">subnets</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_pptp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_qkd:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">qkd</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ssl_client:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">client</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ssl_settings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpn_ssl_settings_authenticationrule:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">authentication-rule</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpnsslweb_userbookmark:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">user-bookmark</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpnsslweb_userbookmark_bookmarks:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">bookmarks</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">user-bookmark</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpnsslweb_userbookmark_bookmarks_formdata:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">bookmarks</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">form-data</span></li>
            <li><span class="li-normal">user-bookmark</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpnsslweb_usergroupbookmark:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">user-group-bookmark</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpnsslweb_usergroupbookmark_bookmarks:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">bookmarks</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">user-group-bookmark</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for vpnsslweb_usergroupbookmark_bookmarks_formdata:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">bookmarks</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">form-data</span></li>
            <li><span class="li-normal">user-group-bookmark</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wanopt_cacheservice:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for wanopt_cacheservice_dstpeer:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">dst-peer</span></li>
        </ul>
        <li><span class="li-normal">params for wanopt_cacheservice_srcpeer:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">src-peer</span></li>
        </ul>
        <li><span class="li-normal">params for wanopt_contentdeliverynetworkrule:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">content-delivery-network-rule</span></li>
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for wanopt_contentdeliverynetworkrule_rules:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">content-delivery-network-rule</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">rules</span></li>
        </ul>
        <li><span class="li-normal">params for wanopt_contentdeliverynetworkrule_rules_contentid:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">content-delivery-network-rule</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">rules</span></li>
        </ul>
        <li><span class="li-normal">params for wanopt_contentdeliverynetworkrule_rules_matchentries:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">content-delivery-network-rule</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">match-entries</span></li>
            <li><span class="li-normal">rules</span></li>
        </ul>
        <li><span class="li-normal">params for wanopt_contentdeliverynetworkrule_rules_skipentries:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">content-delivery-network-rule</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">rules</span></li>
            <li><span class="li-normal">skip-entries</span></li>
        </ul>
        <li><span class="li-normal">params for wanopt_remotestorage:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for wanopt_settings:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wanopt_webcache:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for webfilter_fortiguard:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for webfilter_ftgdlocalrisk:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ftgd-local-risk</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for webfilter_ftgdrisklevel:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ftgd-risk-level</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for webfilter_ipsurlfiltercachesetting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for webfilter_ipsurlfiltersetting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for webfilter_ipsurlfiltersetting6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for webfilter_override:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">override</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for webfilter_searchengine:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">search-engine</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for webproxy_debugurl:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">debug-url</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for webproxy_explicit:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for webproxy_explicit_pacpolicy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">pac-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for webproxy_fastfallback:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">fast-fallback</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for webproxy_global:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for webproxy_urlmatch:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">url-match</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_accesscontrollist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">access-control-list</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_accesscontrollist_layer3ipv4rules:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">access-control-list</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">layer3-ipv4-rules</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_accesscontrollist_layer3ipv6rules:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">access-control-list</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">layer3-ipv6-rules</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_apcfgprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">apcfg-profile</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_apcfgprofile_commandlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">apcfg-profile</span></li>
            <li><span class="li-normal">command-list</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_apstatus:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">ap-status</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_arrpprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">arrp-profile</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_bleprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">ble-profile</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_bonjourprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">bonjour-profile</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_bonjourprofile_policylist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">bonjour-profile</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">policy-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_global:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_anqp3gppcellular:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">anqp-3gpp-cellular</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_anqp3gppcellular_mccmnclist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">anqp-3gpp-cellular</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">mcc-mnc-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_anqpipaddresstype:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">anqp-ip-address-type</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_anqpnairealm:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">anqp-nai-realm</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_anqpnairealm_nailist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">anqp-nai-realm</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">nai-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_anqpnairealm_nailist_eapmethod:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">anqp-nai-realm</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">eap-method</span></li>
            <li><span class="li-normal">nai-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_anqpnairealm_nailist_eapmethod_authparam:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">anqp-nai-realm</span></li>
            <li><span class="li-normal">auth-param</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">eap-method</span></li>
            <li><span class="li-normal">nai-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_anqpnetworkauthtype:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">anqp-network-auth-type</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_anqproamingconsortium:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">anqp-roaming-consortium</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_anqproamingconsortium_oilist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">anqp-roaming-consortium</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">oi-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_anqpvenuename:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">anqp-venue-name</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_anqpvenuename_valuelist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">anqp-venue-name</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">value-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_anqpvenueurl:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">anqp-venue-url</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_anqpvenueurl_valuelist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">anqp-venue-url</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">value-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_h2qpadviceofcharge:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">h2qp-advice-of-charge</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_h2qpadviceofcharge_aoclist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">aoc-list</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">h2qp-advice-of-charge</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_h2qpadviceofcharge_aoclist_planinfo:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">aoc-list</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">h2qp-advice-of-charge</span></li>
            <li><span class="li-normal">plan-info</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_h2qpconncapability:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">h2qp-conn-capability</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_h2qpoperatorname:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">h2qp-operator-name</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_h2qpoperatorname_valuelist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">h2qp-operator-name</span></li>
            <li><span class="li-normal">value-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_h2qposuprovider:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">h2qp-osu-provider</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_h2qposuprovider_friendlyname:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">friendly-name</span></li>
            <li><span class="li-normal">h2qp-osu-provider</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_h2qposuprovider_servicedescription:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">h2qp-osu-provider</span></li>
            <li><span class="li-normal">service-description</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_h2qposuprovidernai:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">h2qp-osu-provider-nai</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_h2qposuprovidernai_nailist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">h2qp-osu-provider-nai</span></li>
            <li><span class="li-normal">nai-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_h2qptermsandconditions:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">h2qp-terms-and-conditions</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_h2qpwanmetric:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">h2qp-wan-metric</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_hsprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">hs-profile</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_icon:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">icon</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_icon_iconlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">icon</span></li>
            <li><span class="li-normal">icon-list</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_qosmap:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">qos-map</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_qosmap_dscpexcept:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">dscp-except</span></li>
            <li><span class="li-normal">qos-map</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_hotspot20_qosmap_dscprange:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">dscp-range</span></li>
            <li><span class="li-normal">qos-map</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_intercontroller:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_intercontroller_intercontrollerpeer:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">inter-controller-peer</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_log:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_mpskprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">mpsk-profile</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_mpskprofile_mpskgroup:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">mpsk-group</span></li>
            <li><span class="li-normal">mpsk-profile</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_mpskprofile_mpskgroup_mpskkey:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">mpsk-group</span></li>
            <li><span class="li-normal">mpsk-key</span></li>
            <li><span class="li-normal">mpsk-profile</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_nacprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">nac-profile</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_qosprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">qos-profile</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_region:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">region</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_setting:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_setting_offendingssid:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">offending-ssid</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_snmp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_snmp_community:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">community</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_snmp_community_hosts:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">community</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">hosts</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_snmp_user:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">user</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_ssidpolicy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ssid-policy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_syslogprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">syslog-profile</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_timers:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_utmprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">utm-profile</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_vap:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vap</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_vap_dynamicmapping:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vap</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_vap_macfilterlist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">mac-filter-list</span></li>
            <li><span class="li-normal">vap</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_vap_mpskkey:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">mpsk-key</span></li>
            <li><span class="li-normal">vap</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_vap_portalmessageoverrides:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vap</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_vap_vlanname:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vap</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">vlan-name</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_vap_vlanpool:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vap</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">vlan-pool</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_vapgroup:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vap-group</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wagprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wag-profile</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_widsprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wids-profile</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtp:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtp_lan:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtp_radio1:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtp_radio2:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtp_radio3:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtp_radio4:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtp_splittunnelingacl:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">split-tunneling-acl</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtpgroup:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp-group</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtpprofile:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp-profile</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtpprofile_denymaclist:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">deny-mac-list</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp-profile</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtpprofile_eslsesdongle:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp-profile</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtpprofile_lan:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp-profile</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtpprofile_lbs:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp-profile</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtpprofile_platform:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp-profile</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtpprofile_radio1:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp-profile</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtpprofile_radio2:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp-profile</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtpprofile_radio3:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp-profile</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtpprofile_radio4:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp-profile</span></li>
        </ul>
        <li><span class="li-normal">params for wireless_wtpprofile_splittunnelingacl:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">split-tunneling-acl</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">wtp-profile</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_reverseconnector:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">reverse-connector</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_trafficforwardproxy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">traffic-forward-proxy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_trafficforwardproxy_quic:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">traffic-forward-proxy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_trafficforwardproxy_sslciphersuites:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ssl-cipher-suites</span></li>
            <li><span class="li-normal">traffic-forward-proxy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_trafficforwardproxy_sslserverciphersuites:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ssl-server-cipher-suites</span></li>
            <li><span class="li-normal">traffic-forward-proxy</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_trafficforwardproxyreverseservice:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_trafficforwardproxyreverseservice_remoteservers:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">remote-servers</span></li>
            <li><span class="li-normal">vdom</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_webportal:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">web-portal</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_webportalbookmark:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">web-portal-bookmark</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_webportalbookmark_bookmarks:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">bookmarks</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">web-portal-bookmark</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_webproxy:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">web-proxy</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_webproxy_apigateway:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">api-gateway</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">web-proxy</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_webproxy_apigateway6:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">api-gateway6</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">web-proxy</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_webproxy_apigateway6_quic:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">api-gateway6</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">web-proxy</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_webproxy_apigateway6_realservers:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">api-gateway6</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">realservers</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">web-proxy</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_webproxy_apigateway6_sslciphersuites:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">api-gateway6</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ssl-cipher-suites</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">web-proxy</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_webproxy_apigateway_quic:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">api-gateway</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">web-proxy</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_webproxy_apigateway_realservers:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">api-gateway</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">realservers</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">web-proxy</span></li>
        </ul>
        <li><span class="li-normal">params for ztna_webproxy_apigateway_sslciphersuites:</span></li>
        <ul class="ul-self">
            <li><span class="li-normal">api-gateway</span></li>
            <li><span class="li-normal">device</span></li>
            <li><span class="li-normal">ssl-cipher-suites</span></li>
            <li><span class="li-normal">vdom</span></li>
            <li><span class="li-normal">web-proxy</span></li>
        </ul>
  </ul>
  </div>
  </section>
  <li><span class="li-head">extra_params</span> Extra parameters. <span class="li-normal">type: dict</span> <span class="li-required">required: false</span></li>
 </ul>
 </ul>
 </ul>






Notes
-----
.. note::

   - Running in workspace locking mode is supported in this FortiManager module, the top level parameters workspace_locking_adom and workspace_locking_timeout help do the work.

   - Selector is a mandatory parameter for the module, and the params is varying depending on the selector.

   - Parameter ``adom`` can be ``null`` or ``''`` for all administrative domains,  ``global`` for global domain and any other custom domain strings. and a particular fact may not support all kinds of domains.

   - In parameters section, ``null`` and ``''`` are identical if you are fetching all objects under that selector category.

   - Normally, running one module can fail when a non-zero rc is returned. you can also override the conditions to fail or succeed with parameters ``rc_failed`` and ``rc_succeeded``

Examples
--------

.. code-block:: yaml+jinja

  - name: Gathering fortimanager device facts
    hosts: fortimanagers
    connection: httpapi
    vars:
      device_name: "XXXXXXX"
      vdom_name: "root"
    tasks:
      - name: Gathering fortimanager device fact
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


Return Values
-------------


Common return values are documented: https://docs.ansible.com/ansible/latest/reference_appendices/common_return_values.html#common-return-values, the following are the fields unique to this module:


.. raw:: html

 <ul>
 <li> <span class="li-return">meta</span> - The result of the request.<span class="li-normal">returned: always</span> <span class="li-normal">type: dict</span></li>
 <ul class="ul-self"> <li> <span class="li-return">request_url</span> - The full url requested. <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: /sys/login/user</span></li>
 <li> <span class="li-return">response_code</span> - The status of api request. <span class="li-normal">returned: always</span> <span class="li-normal">type: int</span> <span class="li-normal">sample: 0</span></li>
 <li> <span class="li-return">response_data</span> - The data body of the api response. <span class="li-normal">returned: optional</span> <span class="li-normal">type: list or dict</span></li>
 <li> <span class="li-return">response_message</span> - The descriptive message of the api response. <span class="li-normal">returned: always</span> <span class="li-normal">type: str</span> <span class="li-normal">sample: OK</span></li>
 <li> <span class="li-return">system_information</span> - The information of the target system. <span class="li-normal">returned: always</span> <span class="li-normal">type: dict</span></li>
 </ul>
 <li> <span class="li-return">rc</span> - The status the request. <span class="li-normal">returned: always</span> <span class="li-normal">type: int</span> <span class="li-normal">0</li>
 <li> <span class="li-return">version_check_warning</span> - Warning if the parameters used in the playbook are not supported by the current FortiManager version. <span class="li-normal">returned: if at least on parameter mpt supported by the current FortiManager version</span> <span class="li-normal">type: list</span> <span class="li-normal">0</li>
 </ul>





Status
------

- This module is not guaranteed to have a backwards compatible interface.


Authors
-------

- Xinwei Du (@dux-fortinet)
- Xing Li (@lix-fortinet)
- Jie Xue (@JieX19)
- Link Zheng (@chillancezen)
- Frank Shen (@fshen01)
- Hongbin Lu (@fgtdev-hblu)


.. hint::

    If you notice any issues in this documentation, you can create a pull request to improve it.


