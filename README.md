Final Network Automation Project by Wesley Sigsworth and Christopher Viktora-Croke

This project is a cumulation of all of the things we learned during our Network Automation class with Holly Yuan. With this project we have combined our learnings of Git and Github, Network design and funamental skills, team work, and ansible automation.

We are using two Cisco 4221 Routers and one Cisco 3650 Switch for this project along with a laptop running a Cisco VM that will be used as our Ansible Control Node(ACN).

To run the playbooks you will need to the ansible-playbook command on your VM along with the playbook file name, eg. ansible-playbook 01_verify_connectivity.yml

The playbooks do the following:

  01: This playbook is used to verify that the routers and switch are able to talk to our ACN
  
  02: This playbook is used to do the inital configurations of our routers and switch, such as hostnames, interface descriptions, and login banners
  
  03: This playbook is used to setup eigrp on the routers, advertising networks and creating loopback interfaces
  
  04: This playbook is used to configure VLANs on our routers and switch, in our case it is doing 1 vlan for data, 1 for management, and configuring our trunk port
  
  05: This playbook is uesd to start our services such as a logging server and NTP server
  
  06: This playbook is used to check connectivitiy again and to configure a backup of our routers and switches in the case tha they get deleted/corrupted.
