:source: fmgd_webproxy_global.py

:orphan:

.. _fmgd_webproxy_global:

fmgd_webproxy_global -- Configure Web proxy global settings.
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

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

- ansible-core>=2.16.0


FortiManager Version Compatibility
----------------------------------
.. raw:: html

 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>



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
 <li><span class="li-head">vdom</span> - The parameter in requested url <span class="li-normal">type: str</span> <span class="li-required">required: true</span> </li>
 <li><span class="li-head">webproxy_global</span> - Configure Web proxy global settings. <span class="li-normal">type: dict</span></li>
 <ul class="ul-self">
 <li><span class="li-head">always_learn_client_ip</span> <b>(Alias name: always-learn-client-ip)</b>  Enable/disable learning the clients ip address from headers for every request. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">fast_policy_match</span> <b>(Alias name: fast-policy-match)</b>  Enable/disable fast matching algorithm for explicit and transparent proxy policy. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">forward_proxy_auth</span> <b>(Alias name: forward-proxy-auth)</b>  Enable/disable forwarding proxy authentication headers. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">forward_server_affinity_timeout</span> <b>(Alias name: forward-server-affinity-timeout)</b>  Period of time before the source ips traffic is no longer assigned to the forwarding server (6 - 60 min, default = 30). <span class="li-normal">type: int</span>
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ldap_user_cache</span> <b>(Alias name: ldap-user-cache)</b>  Enable/disable ldap user cache for explicit and transparent proxy user. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">learn_client_ip</span> <b>(Alias name: learn-client-ip)</b>  Enable/disable learning the clients ip address from headers. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable, traffic-process, log-only]</span>
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">learn_client_ip_from_header</span> <b>(Alias name: learn-client-ip-from-header)</b>  Learn client ip address from the specified headers. <span class="li-normal">type: list</span> <span class="li-normal">choices: [true-client-ip, x-real-ip, x-forwarded-for]</span>
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">learn_client_ip_srcaddr</span> <b>(Alias name: learn-client-ip-srcaddr)</b>  Source address name (srcaddr or srcaddr6 must be set). <span class="li-normal">type: list</span>
 <a id='label14' href="javascript:ContentClick('label15', 'label14');" onmouseover="ContentPreview('label15');" onmouseout="ContentUnpreview('label15');" title="click to collapse or expand..."> more... </a>
 <div id="label15" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">learn_client_ip_srcaddr6</span> <b>(Alias name: learn-client-ip-srcaddr6)</b>  Ipv6 source address name (srcaddr or srcaddr6 must be set). <span class="li-normal">type: list</span>
 <a id='label16' href="javascript:ContentClick('label17', 'label16');" onmouseover="ContentPreview('label17');" onmouseout="ContentUnpreview('label17');" title="click to collapse or expand..."> more... </a>
 <div id="label17" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">log_app_id</span> <b>(Alias name: log-app-id)</b>  Enable/disable always log application type in traffic log. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label18' href="javascript:ContentClick('label19', 'label18');" onmouseover="ContentPreview('label19');" onmouseout="ContentUnpreview('label19');" title="click to collapse or expand..."> more... </a>
 <div id="label19" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">log_forward_server</span> <b>(Alias name: log-forward-server)</b>  Enable/disable forward server name logging in forward traffic log. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label20' href="javascript:ContentClick('label21', 'label20');" onmouseover="ContentPreview('label21');" onmouseout="ContentUnpreview('label21');" title="click to collapse or expand..."> more... </a>
 <div id="label21" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">log_policy_pending</span> <b>(Alias name: log-policy-pending)</b>  Enable/disable logging sessions that are pending on policy matching. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label22' href="javascript:ContentClick('label23', 'label22');" onmouseover="ContentPreview('label23');" onmouseout="ContentUnpreview('label23');" title="click to collapse or expand..."> more... </a>
 <div id="label23" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">max_message_length</span> <b>(Alias name: max-message-length)</b>  Maximum length of http message, not including body (16 - 256 kbytes, default = 32). <span class="li-normal">type: int</span>
 <a id='label24' href="javascript:ContentClick('label25', 'label24');" onmouseover="ContentPreview('label25');" onmouseout="ContentUnpreview('label25');" title="click to collapse or expand..."> more... </a>
 <div id="label25" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">max_request_length</span> <b>(Alias name: max-request-length)</b>  Maximum length of http request line (2 - 64 kbytes, default = 8). <span class="li-normal">type: int</span>
 <a id='label26' href="javascript:ContentClick('label27', 'label26');" onmouseover="ContentPreview('label27');" onmouseout="ContentUnpreview('label27');" title="click to collapse or expand..."> more... </a>
 <div id="label27" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">max_waf_body_cache_length</span> <b>(Alias name: max-waf-body-cache-length)</b>  Maximum length of http messages processed by web application firewall (waf) (10 - 1024 kbytes, default = 32). <span class="li-normal">type: int</span>
 <a id='label28' href="javascript:ContentClick('label29', 'label28');" onmouseover="ContentPreview('label29');" onmouseout="ContentUnpreview('label29');" title="click to collapse or expand..."> more... </a>
 <div id="label29" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">policy_category_deep_inspect</span> <b>(Alias name: policy-category-deep-inspect)</b>  Enable/disable deep inspection for application level category policy matching. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label30' href="javascript:ContentClick('label31', 'label30');" onmouseover="ContentPreview('label31');" onmouseout="ContentUnpreview('label31');" title="click to collapse or expand..."> more... </a>
 <div id="label31" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">proxy_fqdn</span> <b>(Alias name: proxy-fqdn)</b>  Fully qualified domain name (fqdn) that clients connect to (default = default. <span class="li-normal">type: str</span>
 <a id='label32' href="javascript:ContentClick('label33', 'label32');" onmouseover="ContentPreview('label33');" onmouseout="ContentUnpreview('label33');" title="click to collapse or expand..."> more... </a>
 <div id="label33" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">proxy_transparent_cert_inspection</span> <b>(Alias name: proxy-transparent-cert-inspection)</b>  Enable/disable transparent proxy certificate inspection. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label34' href="javascript:ContentClick('label35', 'label34');" onmouseover="ContentPreview('label35');" onmouseout="ContentUnpreview('label35');" title="click to collapse or expand..."> more... </a>
 <div id="label35" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">src_affinity_exempt_addr</span> <b>(Alias name: src-affinity-exempt-addr)</b>  Ipv4 source addresses to exempt proxy affinity. <span class="li-normal">type: list</span>
 <a id='label36' href="javascript:ContentClick('label37', 'label36');" onmouseover="ContentPreview('label37');" onmouseout="ContentUnpreview('label37');" title="click to collapse or expand..."> more... </a>
 <div id="label37" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">src_affinity_exempt_addr6</span> <b>(Alias name: src-affinity-exempt-addr6)</b>  Ipv6 source addresses to exempt proxy affinity. <span class="li-normal">type: list</span>
 <a id='label38' href="javascript:ContentClick('label39', 'label38');" onmouseover="ContentPreview('label39');" onmouseout="ContentUnpreview('label39');" title="click to collapse or expand..."> more... </a>
 <div id="label39" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ssl_ca_cert</span> <b>(Alias name: ssl-ca-cert)</b>  Ssl ca certificate for ssl interception. <span class="li-normal">type: list</span>
 <a id='label40' href="javascript:ContentClick('label41', 'label40');" onmouseover="ContentPreview('label41');" onmouseout="ContentUnpreview('label41');" title="click to collapse or expand..."> more... </a>
 <div id="label41" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ssl_cert</span> <b>(Alias name: ssl-cert)</b>  Ssl certificate for ssl interception. <span class="li-normal">type: list</span>
 <a id='label42' href="javascript:ContentClick('label43', 'label42');" onmouseover="ContentPreview('label43');" onmouseout="ContentUnpreview('label43');" title="click to collapse or expand..."> more... </a>
 <div id="label43" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">strict_web_check</span> <b>(Alias name: strict-web-check)</b>  Enable/disable strict web checking to block web sites that send incorrect headers that dont conform to http 1. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label44' href="javascript:ContentClick('label45', 'label44');" onmouseover="ContentPreview('label45');" onmouseout="ContentUnpreview('label45');" title="click to collapse or expand..."> more... </a>
 <div id="label45" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">webproxy_profile</span> <b>(Alias name: webproxy-profile)</b>  Name of the web proxy profile to apply when explicit proxy traffic is allowed by default and traffic is accepted that does not match an explicit proxy policy. <span class="li-normal">type: list</span>
 <a id='label46' href="javascript:ContentClick('label47', 'label46');" onmouseover="ContentPreview('label47');" onmouseout="ContentUnpreview('label47');" title="click to collapse or expand..."> more... </a>
 <div id="label47" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">tunnel_non_http</span> <b>(Alias name: tunnel-non-http)</b>  Enable/disable allowing non-http traffic. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label48' href="javascript:ContentClick('label49', 'label48');" onmouseover="ContentPreview('label49');" onmouseout="ContentUnpreview('label49');" title="click to collapse or expand..."> more... </a>
 <div id="label49" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> v7.6.2</code></p>
 </div>
 </li>
 <li><span class="li-head">unknown_http_version</span> <b>(Alias name: unknown-http-version)</b>  Action to take when an unknown version of http is encountered: reject, allow (tunnel), or proceed with best-effort. <span class="li-normal">type: str</span> <span class="li-normal">choices: [best-effort, reject, tunnel]</span>
 <a id='label50' href="javascript:ContentClick('label51', 'label50');" onmouseover="ContentPreview('label51');" onmouseout="ContentUnpreview('label51');" title="click to collapse or expand..."> more... </a>
 <div id="label51" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.2.6 -> v7.2.12</code>, <code class="docutils literal notranslate">v7.4.3 -> v7.6.2</code></p>
 </div>
 </li>
 <li><span class="li-head">request_obs_fold</span> <b>(Alias name: request-obs-fold)</b>  Action when http/1. <span class="li-normal">type: str</span> <span class="li-normal">choices: [block, replace-with-sp, keep]</span>
 <a id='label52' href="javascript:ContentClick('label53', 'label52');" onmouseover="ContentPreview('label53');" onmouseout="ContentUnpreview('label53');" title="click to collapse or expand..."> more... </a>
 <div id="label53" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.4 -> v7.4.10</code>, <code class="docutils literal notranslate">v7.6.2 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">http2_client_window_size</span> <b>(Alias name: http2-client-window-size)</b>  Http/2 client initial window size in bytes (65535 - 2147483647, default = 1048576 (1mb)). <span class="li-normal">type: int</span>
 <a id='label54' href="javascript:ContentClick('label55', 'label54');" onmouseover="ContentPreview('label55');" onmouseout="ContentUnpreview('label55');" title="click to collapse or expand..."> more... </a>
 <div id="label55" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.6.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">http2_server_window_size</span> <b>(Alias name: http2-server-window-size)</b>  Http/2 server initial window size in bytes (65535 - 2147483647, default = 1048576 (1mb)). <span class="li-normal">type: int</span>
 <a id='label56' href="javascript:ContentClick('label57', 'label56');" onmouseover="ContentPreview('label57');" onmouseout="ContentUnpreview('label57');" title="click to collapse or expand..."> more... </a>
 <div id="label57" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.6.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">explicit_outgoing_ip</span> <b>(Alias name: explicit-outgoing-ip)</b>  Outgoing http requests by explicit webproxy will have this ip address as their source address. <span class="li-normal">type: list</span>
 <a id='label58' href="javascript:ContentClick('label59', 'label58');" onmouseover="ContentPreview('label59');" onmouseout="ContentUnpreview('label59');" title="click to collapse or expand..."> more... </a>
 <div id="label59" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.8 -> v7.4.10</code>, <code class="docutils literal notranslate">v7.6.4 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">explicit_outgoing_ip6</span> <b>(Alias name: explicit-outgoing-ip6)</b>  Outgoing http requests by explicit webproxy will leave this ip. <span class="li-normal">type: list</span>
 <a id='label60' href="javascript:ContentClick('label61', 'label60');" onmouseover="ContentPreview('label61');" onmouseout="ContentUnpreview('label61');" title="click to collapse or expand..."> more... </a>
 <div id="label61" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.8 -> v7.4.10</code>, <code class="docutils literal notranslate">v7.6.4 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">extended_log</span> <b>(Alias name: extended-log)</b>  Extended log. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label62' href="javascript:ContentClick('label63', 'label62');" onmouseover="ContentPreview('label63');" onmouseout="ContentUnpreview('label63');" title="click to collapse or expand..."> more... </a>
 <div id="label63" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.8 -> v7.4.10</code>, <code class="docutils literal notranslate">v7.6.4 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">https_replacement_message</span> <b>(Alias name: https-replacement-message)</b>  Default action to enable or disable return replacement message for https requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label64' href="javascript:ContentClick('label65', 'label64');" onmouseover="ContentPreview('label65');" onmouseout="ContentUnpreview('label65');" title="click to collapse or expand..."> more... </a>
 <div id="label65" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.8 -> v7.4.10</code>, <code class="docutils literal notranslate">v7.6.4 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">log_http_transaction</span> <b>(Alias name: log-http-transaction)</b>  Log http transaction. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable, all, utm]</span>
 <a id='label66' href="javascript:ContentClick('label67', 'label66');" onmouseover="ContentPreview('label67');" onmouseout="ContentUnpreview('label67');" title="click to collapse or expand..."> more... </a>
 <div id="label67" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.8 -> v7.4.10</code>, <code class="docutils literal notranslate">v7.6.4 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">message_upon_server_error</span> <b>(Alias name: message-upon-server-error)</b>  Enable/disable return of replacement message upon server error detection. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label68' href="javascript:ContentClick('label69', 'label68');" onmouseover="ContentPreview('label69');" onmouseout="ContentUnpreview('label69');" title="click to collapse or expand..."> more... </a>
 <div id="label69" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.8 -> v7.4.10</code>, <code class="docutils literal notranslate">v7.6.4 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">realm</span> Authentication realm. <span class="li-normal">type: str</span>
 <a id='label70' href="javascript:ContentClick('label71', 'label70');" onmouseover="ContentPreview('label71');" onmouseout="ContentUnpreview('label71');" title="click to collapse or expand..."> more... </a>
 <div id="label71" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.8 -> v7.4.10</code>, <code class="docutils literal notranslate">v7.6.4 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">strict_guest</span> <b>(Alias name: strict-guest)</b>  Enable/disable strict guest user checking by the explicit web proxy. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label72' href="javascript:ContentClick('label73', 'label72');" onmouseover="ContentPreview('label73');" onmouseout="ContentUnpreview('label73');" title="click to collapse or expand..."> more... </a>
 <div id="label73" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.8 -> v7.4.10</code>, <code class="docutils literal notranslate">v7.6.4 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">trace_auth_no_rsp</span> <b>(Alias name: trace-auth-no-rsp)</b>  Enable/disable logging timed-out authentication requests. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label74' href="javascript:ContentClick('label75', 'label74');" onmouseover="ContentPreview('label75');" onmouseout="ContentUnpreview('label75');" title="click to collapse or expand..."> more... </a>
 <div id="label75" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.8 -> v7.4.10</code>, <code class="docutils literal notranslate">v7.6.4 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">use_dynamic_pkey</span> <b>(Alias name: use-dynamic-pkey)</b>  Use dynamic pkey. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label76' href="javascript:ContentClick('label77', 'label76');" onmouseover="ContentPreview('label77');" onmouseout="ContentUnpreview('label77');" title="click to collapse or expand..."> more... </a>
 <div id="label77" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.8 -> v7.4.10</code>, <code class="docutils literal notranslate">v7.6.4 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">address_ip_rating</span> <b>(Alias name: address-ip-rating)</b>  Address ip rating. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label78' href="javascript:ContentClick('label79', 'label78');" onmouseover="ContentPreview('label79');" onmouseout="ContentUnpreview('label79');" title="click to collapse or expand..."> more... </a>
 <div id="label79" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.8 -> v7.4.10</code>, <code class="docutils literal notranslate">v7.6.4 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">policy_partial_match</span> <b>(Alias name: policy-partial-match)</b>  Policy partial match. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span>
 <a id='label80' href="javascript:ContentClick('label81', 'label80');" onmouseover="ContentPreview('label81');" onmouseout="ContentUnpreview('label81');" title="click to collapse or expand..."> more... </a>
 <div id="label81" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.9 -> v7.4.10</code>, <code class="docutils literal notranslate">v7.6.5 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">auth_sign_timeout</span> <b>(Alias name: auth-sign-timeout)</b>  Proxy auth query sign timeout in seconds (30 - 3600, default = 120). <span class="li-normal">type: int</span>
 <a id='label82' href="javascript:ContentClick('label83', 'label82');" onmouseover="ContentPreview('label83');" onmouseout="ContentUnpreview('label83');" title="click to collapse or expand..."> more... </a>
 <div id="label83" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.6.5 -> latest</code></p>
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
    gather_facts: false
    vars:
      ansible_httpapi_use_ssl: true
      ansible_httpapi_validate_certs: false
      ansible_httpapi_port: 443
    tasks:
      - name: Configure Web proxy global settings.
        fortinet.fmgdevice.fmgd_webproxy_global:
          # bypass_validation: false
          # workspace_locking_adom: <global or your adom name>
          # workspace_locking_timeout: 300
          # rc_succeeded: [0, -2, -3, ...]
          # rc_failed: [-2, -3, ...]
          device: <your own value>
          vdom: <your own value>
          webproxy_global:
            # always_learn_client_ip: <value in [disable, enable]>
            # fast_policy_match: <value in [disable, enable]>
            # forward_proxy_auth: <value in [disable, enable]>
            # forward_server_affinity_timeout: <integer>
            # ldap_user_cache: <value in [disable, enable]>
            # learn_client_ip: <value in [disable, enable, traffic-process, ...]>
            # learn_client_ip_from_header:
            #   - "true-client-ip"
            #   - "x-real-ip"
            #   - "x-forwarded-for"
            # learn_client_ip_srcaddr: <list or string>
            # learn_client_ip_srcaddr6: <list or string>
            # log_app_id: <value in [disable, enable]>
            # log_forward_server: <value in [disable, enable]>
            # log_policy_pending: <value in [disable, enable]>
            # max_message_length: <integer>
            # max_request_length: <integer>
            # max_waf_body_cache_length: <integer>
            # policy_category_deep_inspect: <value in [disable, enable]>
            # proxy_fqdn: <string>
            # proxy_transparent_cert_inspection: <value in [disable, enable]>
            # src_affinity_exempt_addr: <list or string>
            # src_affinity_exempt_addr6: <list or string>
            # ssl_ca_cert: <list or string>
            # ssl_cert: <list or string>
            # strict_web_check: <value in [disable, enable]>
            # webproxy_profile: <list or string>
            # tunnel_non_http: <value in [disable, enable]>
            # unknown_http_version: <value in [best-effort, reject, tunnel]>
            # request_obs_fold: <value in [block, replace-with-sp, keep]>
            # http2_client_window_size: <integer>
            # http2_server_window_size: <integer>
            # explicit_outgoing_ip: <list or string>
            # explicit_outgoing_ip6: <list or string>
            # extended_log: <value in [disable, enable]>
            # https_replacement_message: <value in [disable, enable]>
            # log_http_transaction: <value in [disable, enable, all, ...]>
            # message_upon_server_error: <value in [disable, enable]>
            # realm: <string>
            # strict_guest: <value in [disable, enable]>
            # trace_auth_no_rsp: <value in [disable, enable]>
            # use_dynamic_pkey: <value in [disable, enable]>
            # address_ip_rating: <value in [disable, enable]>
            # policy_partial_match: <value in [disable, enable]>
            # auth_sign_timeout: <integer>


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
