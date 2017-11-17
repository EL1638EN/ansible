jdk8
=========

Install of Java Development Kit (JDK).

Requirements
------------

None.

Role Variables
--------------

| Nom           | Default Value  | Description|
| ------------- |:-------------:|-----------:|
|jdk8_java_version|1.8.0_131|Version du jdk à installer.|
|jdk8_versions|/opt/jdk_versions|Répertoire contenant  les JDKs|
|jdk8_java_home|/opt/jdk_versions/jdk1.8.0_131|Chemin absolu du répertoire où sera installé le JDK 1.8.0_131.|
|jdk8_tarball_name_32|jdk-8u131-linux-i586.tar.gz|Archive .tar.gz pour les machines 32 bits.|
|jdk8_tarball_name_64|jdk-8u131-linux-x64.tar.gz|Archive .tar.gz pour les machines 64 bits.|
|jdk8_32_url|-|URL de téléchargement du JDK pour une machine 32 bits.|
|jdk8_64_url|-|URL de téléchargement du JDK pour une machine 64 bits.|


Dependencies
------------

None.

Example Playbook
----------------

- hosts: servers
  roles:
     - { role: jdk }

License
-------

BSD

Author Information
------------------

Eric Coovi LEGBA.

Resources
------------------