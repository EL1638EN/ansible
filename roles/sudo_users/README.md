sudo_users
=========

sudo_users gives sudo roles to user.

Requirements
------------

None.

Role Variables
--------------


| Name	        | Default Value	| Description|
| ------------- |:-------------:| ----------:|
|user_name| - |User name.|
|user_comment| - |Comment on creation account|
|user_password|*****|User's password|
|user_ssh_key_passphrase|*****|User's private key passphrase|
|user_public_ssh_key|******|SSH public key.|



Dependencies
------------

None.

Example Playbook
----------------

Install sudo_users
```yaml
- hosts: servers
  roles:
    - { role: sudo_users, user_name: "deploy", user_password: "******", user_public_ssh_key: "ssh-rsa AAAAB3NzaC1*********" }
```

License
-------

BSD

Author Information
------------------

Eric LEGBA.