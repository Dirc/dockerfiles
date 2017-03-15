
FROM williamyeh/ansible:centos7-onbuild

MAINTAINER ericor

# ==> Specify requirements filename;  default = "requirements.yml"
#ENV REQUIREMENTS  requirements.yml

# ==> Specify playbook filename;      default = "playbook.yml"
#ENV PLAYBOOK      playbook.yml

# ==> Specify inventory filename;     default = "/etc/ansible/hosts"
#ENV INVENTORY     inventory.ini

# ==> Executing Ansible (with a simple wrapper)...
#RUN ansible-playbook-wrapper
RUN ansible-playbook ./playbook.yml -v -i inventory.ini --connection=local --sudo

