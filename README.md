# Ansible ELK Playbook

This playbook is for setting up version 5.x of the ELK Stack on a remote server.

## Notes and requirements

 - The playbook was built and tested on Amazon Linux EC2, for ELK versions 5.x
 - You will need Ansible installed and running
 - Playbook is currently configured to set up the ELK stack together with Metricbeat for server perf monitoring and Filebeat.

 ## Instructions

 1. In the terminal on the machine hosting Ansible, clone this repo.
 2. Cd into the directory, and run:

```
 ansible-playbook  --become --become-user=root --ask-become-pass --connection=127.0.0.1 site.yml

```

