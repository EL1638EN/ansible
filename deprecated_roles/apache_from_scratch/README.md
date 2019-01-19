apache
=========

apache makes configurations on the Apache server : 
  - download and compile apache archive file
  - right of the directories (owner, group)
  - deploy configuration files
  - enable service to start/stop/reload/restart Apache Server.

Requirements
------------

None.

Role Variables
--------------
 
| Name	        | Default Value	| Description|
| ------------- |:-------------:| ----------:|
|apache_http_default_port|80|HTTP Port|
|apache_https_default_port|443|HTTPS Port|
|apache_home|/opt/apache2|Installation directory for the current version of Apache|
|apache_logs_dir|/var/log/apache2|Directory containing Apache's log files|
|apache_conf_dir|/opt/apache2/conf|Directory containing Apache's configuration files|
|apache_modules_file|/opt/apache2/conf/modules.conf|List of the modules|
|apache_httpd_file|/opt/apache2/conf/httpd.conf|HTTPD configuration file|
|apache_init_script|/etc/init.d/apache|Script to control Apache server (start/stop/restart/reload)|
|apache_root_user|root|Owner of the Apache's directories|
|apache_root_group|sys|Owner's group|
|apache_user|wwwd|Dedicated user to run the httpd daemon|
|apache_user_group|wwwd|Dedicated user's group|
|apache_files|-|List of configuration's files which will be deployed|
|apache_log_level|warn|Log levels|
|apache_max_clients|300|Maximum client|
|apache_keep_alive|On|Keep alive configuration|
|apache_max_keep_alive_requests|150|Max keep alive requests|
|apache_keep_alive_timeout|15|Keep alive timeout|
|apache_goss_enabled|False|Enable(True)/Disable(False) [Goss](https://github.com/aelsabbahy/goss) checking after execution of playbook.|

Dependencies
------------

None.

Example Playbook
----------------

Install apache
```yaml
- hosts: all
  roles:
    - { role: apache }
```

License
-------

BSD

Author Information
------------------
Eric LEGBA.
