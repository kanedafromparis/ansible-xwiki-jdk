Role Name
=========

This is a role in order to install the targeted jdk version

Requirements
------------

- Ansible 2.0
- Debian 7.0+

Role Variables
--------------

### defaults/main.yml

The default should be open-jdk1.7.0
jdk.version : open-jdk1.7
jdk.links : /usr/local/java
jdk.dir : /usr/local/java 

### vars/main.yml
    java_folder: "/usr/lib/jvm"
		java_version: package to install possible values : 
		 - "openjdk-7-jdk"
		 - "oracle-java8-installer"
		java_alias_default: folder of installation, possible values :
		 - "java-7-openjdk-amd64"
		 - "java-8-oracle"


NTR (nothing to report)

Dependencies
------------

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers 
      vars:
        java_versions: oracle-jdk7-installer  			
      roles:      
      - {role: ansible-xwiki-jdk}
      

License
-------

BSD

Author Information
------------------
C. Sabourdin inspire by Git-hub
