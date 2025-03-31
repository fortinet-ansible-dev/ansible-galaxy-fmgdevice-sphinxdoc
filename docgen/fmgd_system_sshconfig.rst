:source: fmgd_system_sshconfig.py

:orphan:

.. _fmgd_system_sshconfig:

fmgd_system_sshconfig -- Configure SSH config.
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


FortiManager Version Compatibility
----------------------------------
.. raw:: html

 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>



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
 <li><span class="li-head">system_sshconfig</span> - Configure SSH config. <span class="li-normal">type: dict</span></li>
 <ul class="ul-self">
 <li><span class="li-head">ssh_enc_algo</span> <b>(Alias name: ssh-enc-algo)</b>  Select one or more ssh ciphers. <span class="li-normal">type: list</span> <span class="li-normal">choices: [chacha20-poly1305@openssh.com, aes128-ctr, aes192-ctr, aes256-ctr, arcfour256, arcfour128, aes128-cbc, 3des-cbc, blowfish-cbc, cast128-cbc, aes192-cbc, aes256-cbc, arcfour, rijndael-cbc@lysator.liu.se, aes128-gcm@openssh.com, aes256-gcm@openssh.com]</span> 
 <a id='label0' href="javascript:ContentClick('label1', 'label0');" onmouseover="ContentPreview('label1');" onmouseout="ContentUnpreview('label1');" title="click to collapse or expand..."> more... </a>
 <div id="label1" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ssh_hsk</span> <b>(Alias name: ssh-hsk)</b>  Config ssh host key. <span class="li-normal">type: str</span>
 <a id='label2' href="javascript:ContentClick('label3', 'label2');" onmouseover="ContentPreview('label3');" onmouseout="ContentUnpreview('label3');" title="click to collapse or expand..."> more... </a>
 <div id="label3" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ssh_hsk_algo</span> <b>(Alias name: ssh-hsk-algo)</b>  Select one or more ssh hostkey algorithms. <span class="li-normal">type: list</span> <span class="li-normal">choices: [ssh-rsa, ecdsa-sha2-nistp521, rsa-sha2-256, rsa-sha2-512, ssh-ed25519, ecdsa-sha2-nistp384, ecdsa-sha2-nistp256]</span> 
 <a id='label4' href="javascript:ContentClick('label5', 'label4');" onmouseover="ContentPreview('label5');" onmouseout="ContentUnpreview('label5');" title="click to collapse or expand..."> more... </a>
 <div id="label5" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ssh_hsk_override</span> <b>(Alias name: ssh-hsk-override)</b>  Enable/disable ssh host key override in ssh daemon. <span class="li-normal">type: str</span> <span class="li-normal">choices: [disable, enable]</span> 
 <a id='label6' href="javascript:ContentClick('label7', 'label6');" onmouseover="ContentPreview('label7');" onmouseout="ContentUnpreview('label7');" title="click to collapse or expand..."> more... </a>
 <div id="label7" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ssh_hsk_password</span> <b>(Alias name: ssh-hsk-password)</b>  Password for ssh-hostkey. <span class="li-normal">type: list</span>
 <a id='label8' href="javascript:ContentClick('label9', 'label8');" onmouseover="ContentPreview('label9');" onmouseout="ContentUnpreview('label9');" title="click to collapse or expand..."> more... </a>
 <div id="label9" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ssh_kex_algo</span> <b>(Alias name: ssh-kex-algo)</b>  Select one or more ssh kex algorithms. <span class="li-normal">type: list</span> <span class="li-normal">choices: [diffie-hellman-group1-sha1, diffie-hellman-group14-sha1, diffie-hellman-group-exchange-sha1, diffie-hellman-group-exchange-sha256, curve25519-sha256@libssh.org, ecdh-sha2-nistp256, ecdh-sha2-nistp384, ecdh-sha2-nistp521, diffie-hellman-group14-sha256, diffie-hellman-group16-sha512, diffie-hellman-group18-sha512]</span> 
 <a id='label10' href="javascript:ContentClick('label11', 'label10');" onmouseover="ContentPreview('label11');" onmouseout="ContentUnpreview('label11');" title="click to collapse or expand..."> more... </a>
 <div id="label11" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
 </div>
 </li>
 <li><span class="li-head">ssh_mac_algo</span> <b>(Alias name: ssh-mac-algo)</b>  Select one or more ssh mac algorithms. <span class="li-normal">type: list</span> <span class="li-normal">choices: [hmac-md5, hmac-md5-etm@openssh.com, hmac-md5-96, hmac-md5-96-etm@openssh.com, hmac-sha1, hmac-sha1-etm@openssh.com, hmac-sha2-256, hmac-sha2-256-etm@openssh.com, hmac-sha2-512, hmac-sha2-512-etm@openssh.com, hmac-ripemd160, hmac-ripemd160@openssh.com, hmac-ripemd160-etm@openssh.com, umac-64@openssh.com, umac-128@openssh.com, umac-64-etm@openssh.com, umac-128-etm@openssh.com]</span> 
 <a id='label12' href="javascript:ContentClick('label13', 'label12');" onmouseover="ContentPreview('label13');" onmouseout="ContentUnpreview('label13');" title="click to collapse or expand..."> more... </a>
 <div id="label13" style="display:none">
 <p>Supported Version Ranges: <code class="docutils literal notranslate">v7.4.3 -> latest</code></p>
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
      - name: Configure SSH config.
        fortinet.fmgdevice.fmgd_system_sshconfig:
          # bypass_validation: false
          workspace_locking_adom: <value in [global, custom adom including root]>
          workspace_locking_timeout: 300
          # rc_succeeded: [0, -2, -3, ...]
          # rc_failed: [-2, -3, ...]
          device: <your own value>
          system_sshconfig:
            # ssh_enc_algo:
            #   - "chacha20-poly1305@openssh.com"
            #   - "aes128-ctr"
            #   - "aes192-ctr"
            #   - "aes256-ctr"
            #   - "arcfour256"
            #   - "arcfour128"
            #   - "aes128-cbc"
            #   - "3des-cbc"
            #   - "blowfish-cbc"
            #   - "cast128-cbc"
            #   - "aes192-cbc"
            #   - "aes256-cbc"
            #   - "arcfour"
            #   - "rijndael-cbc@lysator.liu.se"
            #   - "aes128-gcm@openssh.com"
            #   - "aes256-gcm@openssh.com"
            # ssh_hsk: <string>
            # ssh_hsk_algo:
            #   - "ssh-rsa"
            #   - "ecdsa-sha2-nistp521"
            #   - "rsa-sha2-256"
            #   - "rsa-sha2-512"
            #   - "ssh-ed25519"
            #   - "ecdsa-sha2-nistp384"
            #   - "ecdsa-sha2-nistp256"
            # ssh_hsk_override: <value in [disable, enable]>
            # ssh_hsk_password: <list or string>
            # ssh_kex_algo:
            #   - "diffie-hellman-group1-sha1"
            #   - "diffie-hellman-group14-sha1"
            #   - "diffie-hellman-group-exchange-sha1"
            #   - "diffie-hellman-group-exchange-sha256"
            #   - "curve25519-sha256@libssh.org"
            #   - "ecdh-sha2-nistp256"
            #   - "ecdh-sha2-nistp384"
            #   - "ecdh-sha2-nistp521"
            #   - "diffie-hellman-group14-sha256"
            #   - "diffie-hellman-group16-sha512"
            #   - "diffie-hellman-group18-sha512"
            # ssh_mac_algo:
            #   - "hmac-md5"
            #   - "hmac-md5-etm@openssh.com"
            #   - "hmac-md5-96"
            #   - "hmac-md5-96-etm@openssh.com"
            #   - "hmac-sha1"
            #   - "hmac-sha1-etm@openssh.com"
            #   - "hmac-sha2-256"
            #   - "hmac-sha2-256-etm@openssh.com"
            #   - "hmac-sha2-512"
            #   - "hmac-sha2-512-etm@openssh.com"
            #   - "hmac-ripemd160"
            #   - "hmac-ripemd160@openssh.com"
            #   - "hmac-ripemd160-etm@openssh.com"
            #   - "umac-64@openssh.com"
            #   - "umac-128@openssh.com"
            #   - "umac-64-etm@openssh.com"
            #   - "umac-128-etm@openssh.com"


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
