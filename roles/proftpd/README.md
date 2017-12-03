proftp
=========

Installation of ProFTP server.

Requirements
------------

None.

Role Variables
--------------

| Name	        | Default Value	| Description|
| ------------- |:-------------:| ----------:|
|proftpd_version|1.3.5|ProFTP version.|
|proftpd_user|proftpd|ProFTP User.|
|proftpd_user_group|proftpd|ProFTP User group.|
|proftpd_server_name|"Syscom FTP Server"|ProFTP Server name.|
|proftpd_transfert_log_file|/var/log/proftpd/xferlog|Transfert Log absolute path.|
|proftpd_system_log_file|/var/log/proftpd/proftpd.log|System Log absolute path.|
|proftpd_config_file|/etc/proftpd/proftpd.conf|ProFTP main configuration file.|
|proftpd_modules_config_file|/etc/proftpd/modules.conf|ProFTP module configuration file.|
|proftpd_goss_enabled|False|Enable/Disable goss checking after installation.|
|proftpd_default_port|21|ProFTP default port.|
|proftpd_min_passive_port|5000|ProFTP minimum passive port.|
|proftpd_max_passive_port|5100|ProFTP maximum passive port.|
|proftpd_iptables_enabled|False|Enable/Disable iptables rule.|
|proftpd_network_interface|eth0|Network interface where iptables rule will be applied.|
|proftpd_config_directive|List|List of configurations for ProFTP.|


Dependencies
------------

None.

Example Playbook
----------------

Install proftp
```yaml
- hosts: all
  roles:
    - { role: proftp }
```

License
-------

BSD

Author Information
------------------

Eric LEGBA.
