Vsftpd

An Ansible role for installing and configuring vsftpd on CentOS/RHEL 7.

Tasks

tasks/main.yml is the most important file. This is the actual playbook that describes all the actions that must be performed

defaults

defaults/main.yml and vars/main.yml contain variables. In defaults you will find default values for variables that can be adjusted by the user. In vars come those variables that in principle should not be changed, for example the names of packages to be installed.

Handlers

handlers/main.yml contains tasks that must be performed in response to an event. The typical example is restarting a service if you have modified the configuration file. 

meta/main.yml contains meta information about the role, eg author name and license. You should definitely adjust this when you publish your role.  
#
#
Test

tests/ contains a small test environment with its own Vagrant file playbook

Links 

http://vsftpd.beasts.org/vsftpd_conf.html
http://access.redhat.com/documentation/en-US/Red_Hat_Enterprise_Linux/7/html/System_Administrators_Guide/s1-FTP.html

License

MIT
