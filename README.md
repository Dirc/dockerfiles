# Docker files
## Django example
See other github project: django_project
## Ansible server image
Easy way to test your playbook.yml.

### Verify playbook
During building of the image

```
docker build -t ansible/server:v2 .
```

### Run container and verify it's working

```
docker run -it ansible/server:v2 /bin/bash
ansible -m ping -c local -b all
ansible -m shell -a 'echo "Hello World!"' -c local -b all
```
