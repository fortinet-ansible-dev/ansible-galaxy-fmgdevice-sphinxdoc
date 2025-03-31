:source: fmgd_system_np6xlite_fpanomaly.py

:orphan:

.. _fmgd_system_np6xlite_fpanomaly:

fmgd_system_np6xlite_fpanomaly -- NP6XLITE IPv4 anomaly protection.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

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


FortiManager Version Compatibility
----------------------------------
.. raw:: html

 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>



Parameters
----------
.. raw:: html

 <ul>
 <li><span class="li-head">access_token</span> -The token to access FortiManager without using username and password. <span class="li-normal">type: str</span> <span class="li-required">required: false</span></li> <li><span class="li-head">bypass_validation</span> - Only set to True when module schema diffs with FortiManager API structure, module continues to execute without validating parameters. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal"> default: False</span> </li>
 <li><span class="li-head">enable_log</span> - Enable/Disable logging for task. <span class="li-normal">type: bool</span> <span class="li-required">required: false</span> <span class="li-normal"> default: False</span> </li>
 <li><span class="li-head">forticloud_access_token</span> - Access token of forticloud managed API users, this option is available with FortiManager later than 6.4.0. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> </li>
 <li><span class="li-head">proposed_method</span> - The overridden method for the underlying Json RPC request. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal"> choices: set, update, add</span> </li>
 <li><span class="li-head">rc_succeeded</span> - The rc codes list with which the conditions to succeed will be overriden. <span class="li-normal">type: list</span> <span class="li-required">required: false</span> </li>
 <li><span class="li-head">rc_failed</span> - The rc codes list with which the conditions to fail will be overriden. <span class="li-normal">type: list</span> <span class="li-required">required: false</span> </li>
 <li><span class="li-head">workspace_locking_adom</span> - Acquire the workspace lock if FortiManager is running in workspace mode. <span class="li-normal">type: str</span> <span class="li-required">required: false</span> <span class="li-normal"> choices: global, custom adom including root</span> </li>
 <li><span class="li-head">workspace_locking_timeout</span> - The maximum time in seconds to wait for other users to release workspace lock. <span class="li-normal">type: integer</span> <span class="li-required">required: false</span>  <span class="li-normal">default: 300</span> </li>
 <li><span class="li-head">device</span> - The parameter in requested url <span class="li-normal">type: str</span> <span class="li-required">required: true</span> </li>
 <li><span class="li-head">np6xlite</span> - The parameter in requested url <span class="li-normal">type: str</span> <span class="li-required">required: true</span> </li>
 <li><span class="li-head">system_np6xlite_fpanomaly</span> - NP6XLITE IPv4 anomaly protection. <span class="li-normal">type: dict</span></li>
 <ul class="ul-self">
 <li><span class="li-head">icmp_csum_err</span> <b>(Alias name: icmp-csum-err)</b>  Invalid ipv4 icmp checksum anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [drop, trap-to-host]</span> 
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">icmp_frag</span> <b>(Alias name: icmp-frag)</b>  Layer 3 fragmented packets that could be part of layer 4 icmp anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">icmp_land</span> <b>(Alias name: icmp-land)</b>  Icmp land anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv4_csum_err</span> <b>(Alias name: ipv4-csum-err)</b>  Invalid ipv4 ip checksum anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [drop, trap-to-host]</span> 
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv4_land</span> <b>(Alias name: ipv4-land)</b>  Land anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv4_optlsrr</span> <b>(Alias name: ipv4-optlsrr)</b>  Loose source record route option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv4_optrr</span> <b>(Alias name: ipv4-optrr)</b>  Record route option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv4_optsecurity</span> <b>(Alias name: ipv4-optsecurity)</b>  Security option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv4_optssrr</span> <b>(Alias name: ipv4-optssrr)</b>  Strict source record route option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv4_optstream</span> <b>(Alias name: ipv4-optstream)</b>  Stream option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv4_opttimestamp</span> <b>(Alias name: ipv4-opttimestamp)</b>  Timestamp option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv4_proto_err</span> <b>(Alias name: ipv4-proto-err)</b>  Invalid layer 4 protocol anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv4_unknopt</span> <b>(Alias name: ipv4-unknopt)</b>  Unknown option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv6_daddr_err</span> <b>(Alias name: ipv6-daddr-err)</b>  Destination address as unspecified or loopback address anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv6_land</span> <b>(Alias name: ipv6-land)</b>  Land anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv6_optendpid</span> <b>(Alias name: ipv6-optendpid)</b>  End point identification anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv6_opthomeaddr</span> <b>(Alias name: ipv6-opthomeaddr)</b>  Home address option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv6_optinvld</span> <b>(Alias name: ipv6-optinvld)</b>  Invalid option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv6_optjumbo</span> <b>(Alias name: ipv6-optjumbo)</b>  Jumbo options anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv6_optnsap</span> <b>(Alias name: ipv6-optnsap)</b>  Network service access point address option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv6_optralert</span> <b>(Alias name: ipv6-optralert)</b>  Router alert option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv6_opttunnel</span> <b>(Alias name: ipv6-opttunnel)</b>  Tunnel encapsulation limit option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv6_proto_err</span> <b>(Alias name: ipv6-proto-err)</b>  Layer 4 invalid protocol anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv6_saddr_err</span> <b>(Alias name: ipv6-saddr-err)</b>  Source address as multicast anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ipv6_unknopt</span> <b>(Alias name: ipv6-unknopt)</b>  Unknown option anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">tcp_csum_err</span> <b>(Alias name: tcp-csum-err)</b>  Invalid ipv4 tcp checksum anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [drop, trap-to-host]</span> 
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">tcp_fin_noack</span> <b>(Alias name: tcp-fin-noack)</b>  Tcp syn flood with fin flag set without ack setting anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">tcp_fin_only</span> <b>(Alias name: tcp-fin-only)</b>  Tcp syn flood with only fin flag set anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">tcp_land</span> <b>(Alias name: tcp-land)</b>  Tcp land anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">tcp_no_flag</span> <b>(Alias name: tcp-no-flag)</b>  Tcp syn flood with no flag set anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">tcp_syn_data</span> <b>(Alias name: tcp-syn-data)</b>  Tcp syn flood packets with data anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">tcp_syn_fin</span> <b>(Alias name: tcp-syn-fin)</b>  Tcp syn flood syn/fin flag set anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">tcp_winnuke</span> <b>(Alias name: tcp-winnuke)</b>  Tcp winnuke anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">udp_csum_err</span> <b>(Alias name: udp-csum-err)</b>  Invalid ipv4 udp checksum anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [drop, trap-to-host]</span> 
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">udp_land</span> <b>(Alias name: udp-land)</b>  Udp land anomalies. <span class="li-normal">type: str</span> <span class="li-normal">choices: [allow, drop, trap-to-host]</span> 
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.9</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 </ul>
 </ul>



Notes
-----
.. note::
   - Running in workspace locking mode is supported in this FortiManager module, the top level parameters workspace_locking_adom and workspace_locking_timeout help do the work.
   - To create or update an object, use state: present directive.
   - To delete an object, use state: absent directive
   - Normally, running one module can fail when a non-zero rc is returned. you can also override the conditions to fail or succeed with parameters rc_failed and rc_succeeded

Examples
--------

.. code-block:: yaml+jinja

  - name: Example playbook (generated based on argument schema)
    hosts: fortimanagers
    connection: httpapi
    vars:
      ansible_httpapi_use_ssl: true
      ansible_httpapi_validate_certs: false
      ansible_httpapi_port: 443
    tasks:
      - name: NP6XLITE IPv4 anomaly protection.
        fortinet.fmgdevice.fmgd_system_np6xlite_fpanomaly:
          # bypass_validation: false
          workspace_locking_adom: <value in [global, custom adom including root]>
          workspace_locking_timeout: 300
          # rc_succeeded: [0, -2, -3, ...]
          # rc_failed: [-2, -3, ...]
          device: <your own value>
          np6xlite: <your own value>
          system_np6xlite_fpanomaly:
            # icmp_csum_err: <value in [drop, trap-to-host]>
            # icmp_frag: <value in [allow, drop, trap-to-host]>
            # icmp_land: <value in [allow, drop, trap-to-host]>
            # ipv4_csum_err: <value in [drop, trap-to-host]>
            # ipv4_land: <value in [allow, drop, trap-to-host]>
            # ipv4_optlsrr: <value in [allow, drop, trap-to-host]>
            # ipv4_optrr: <value in [allow, drop, trap-to-host]>
            # ipv4_optsecurity: <value in [allow, drop, trap-to-host]>
            # ipv4_optssrr: <value in [allow, drop, trap-to-host]>
            # ipv4_optstream: <value in [allow, drop, trap-to-host]>
            # ipv4_opttimestamp: <value in [allow, drop, trap-to-host]>
            # ipv4_proto_err: <value in [allow, drop, trap-to-host]>
            # ipv4_unknopt: <value in [allow, drop, trap-to-host]>
            # ipv6_daddr_err: <value in [allow, drop, trap-to-host]>
            # ipv6_land: <value in [allow, drop, trap-to-host]>
            # ipv6_optendpid: <value in [allow, drop, trap-to-host]>
            # ipv6_opthomeaddr: <value in [allow, drop, trap-to-host]>
            # ipv6_optinvld: <value in [allow, drop, trap-to-host]>
            # ipv6_optjumbo: <value in [allow, drop, trap-to-host]>
            # ipv6_optnsap: <value in [allow, drop, trap-to-host]>
            # ipv6_optralert: <value in [allow, drop, trap-to-host]>
            # ipv6_opttunnel: <value in [allow, drop, trap-to-host]>
            # ipv6_proto_err: <value in [allow, drop, trap-to-host]>
            # ipv6_saddr_err: <value in [allow, drop, trap-to-host]>
            # ipv6_unknopt: <value in [allow, drop, trap-to-host]>
            # tcp_csum_err: <value in [drop, trap-to-host]>
            # tcp_fin_noack: <value in [allow, drop, trap-to-host]>
            # tcp_fin_only: <value in [allow, drop, trap-to-host]>
            # tcp_land: <value in [allow, drop, trap-to-host]>
            # tcp_no_flag: <value in [allow, drop, trap-to-host]>
            # tcp_syn_data: <value in [allow, drop, trap-to-host]>
            # tcp_syn_fin: <value in [allow, drop, trap-to-host]>
            # tcp_winnuke: <value in [allow, drop, trap-to-host]>
            # udp_csum_err: <value in [drop, trap-to-host]>
            # udp_land: <value in [allow, drop, trap-to-host]>


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
 <li> <span class="li-return">rc</span> - The status the request. <span class="li-normal">returned: always</span> <span class="li-normal">type: int</span> <span class="li-normal">sample: 0</span></li>
 <li> <span class="li-return">version_check_warning</span> - Warning if the parameters used in the playbook are not supported by the current FortiManager version. <span class="li-normal">returned: if at least one parameter not supported by the current FortiManager version</span> <span class="li-normal">type: list</span> </li>
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
