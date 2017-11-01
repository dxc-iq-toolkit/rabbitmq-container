RabbitMQ
=========
[![Build Status](https://travis-ci.org/bingoarun/rabbitmq-container.svg?branch=master)](https://travis-ci.org/bingoarun/rabbitmq-container) [![Ansible Galaxy](https://img.shields.io/badge/galaxy-rabbitmq--container-blue.svg)](https://galaxy.ansible.com/bingoarun/rabbitmq-container/)

Use this role to add a rabbitmq service to your Ansbile container project.

Role Variables
--------------

Set the following environment variables in container.yml:

RABBITMQ_DEFAULT_USER
> RabbitMQ user name. Defaults to `rabbitmq`.

RABBITMQ_DEFAULT_PASSWORD
> RabbitMQ user password. Defaults to `rabbitmq`.

RABBITMQ_GROUP
> RabbitMQ user group. Defaults to `rabbitmq`.

RABBITMQ_DEFAULT_VHOST
> RabbitMQ virtual host. Defaults to `my_vhost`.

RABBITMQ_NODE_PORT
> RabbitMQ service port number. Defautls to `5672`

RABBITMQ_ADMIN_USER
> RabbitMQ administrator user name. Defaults to `admin`.

RABBITMQ_ADMIN_PASSWORD
> RabbitMQ administrator password. Defaults to `ChangeMe!`.

Equivalent variables are set in defaults/main.yml and can be overriden at execution time.

Dependencies
------------

None

Example playbook
----------------

Run the following commands to install the service

```
# Set the working directory to your Ansible Container project root
$ cd myproject

# Install the service
$ ansible-container install bingoarun.rabbitmq-container
```


```
- hosts: server
  roles:
    - { role: bingoarun.rabbitmq-container }
```

License
-------

MIT

Author Information
------------------

Arun prasath - [@bingoarun](https://github.com/bingoarun)
