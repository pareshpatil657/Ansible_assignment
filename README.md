#Tomcat8 and Apache web server deployment

Prerequisite:

1. Tested on Ansible 2.4.3
2. Expects Ubuntu 16.04

Contents:
1. playbook.yml file
2. Apps folder which contains a sample war.
3. Template folder which contains configuration files for:
     1. Set Tomcat8 as default service
     2. VirtualHost file


These playbook deploys a very basic implementation of Tomcat8 Application server and Apache web server. To use them, first edit the "hosts" inventory file to contain the hostnames of the machines on which you want Tocmat and web server to be deployed.

To run the playbook:

ansible-playbook playbook.yml -b

When the playbook run completes, you should be able to see the Tomcat8 Application Server running and Apache as front ending web server on the ports 80, on the target machines.
