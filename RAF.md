
1°) Gérer tous les mots de passe avec Ansible-Vault.
Les rôles impactés seraient : Apache, Tomcat, SonarQube, Nexus, postgres_instance, monit

2°) Créer un repertoire /var/logs/tomcat qui va contenir les logs d'Apache Tomcat

3°)Faire un playbook contenant tous les rôles pour initialiser un serveur dédié from scratch

4°) Faire la documentation d'installation pour : 
 - JDK, Maven, Gradle
 - Proftpd
 - etc..
 Il faut refaire ces docs d'installation améliorés avec Gitbook

 5°) Faire la configuration Apache Mod Proxy pour les serveurs Nexus et SonarQube