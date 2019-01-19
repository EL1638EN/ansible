postgres_instance
=========

postgres_instance adds users, databases and schemas to PostgreSQL.

Requirements
------------

None.

Role Variables
--------------

| Name	        | Default Value	| Description|
| ------------- |:-------------:| ----------:|
|dbs|-|List of users, databases and schemas.|


Dependencies
------------

None.

Example Playbook
----------------

Install postgres_instance
```yaml
- hosts: servers
  roles:
    - { role: postgres_instance }
```

License
-------

BSD

Author Information
------------------

Eric LEGBA.