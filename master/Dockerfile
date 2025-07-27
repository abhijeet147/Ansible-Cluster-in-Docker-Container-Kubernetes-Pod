
FROM alpine:latest

RUN apk update && apk add --no-cache python3 py3-pip openssh ansible

RUN mkdir /etc/ansible

COPY ansible.cfg /etc/ansible/ansible.cfg
COPY inventory /etc/ansible/hosts
COPY playbook.yml /root/playbook.yml

CMD ["/bin/sh"]
