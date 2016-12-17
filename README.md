Role Name
=========

Use this role to add a rabbitmq service to your Ansbile container project.


Role Variables
--------------

Set the following environment variables in container.yml:

RABBITMQ_DEFAULT_USER
> RabbitMQ user name. Defaults to `rabbimq`.

RABBITMQ_GROUP
> RabbitMQ user group. Defaults to `rabbitmq`.

RABBITMQ_DEFAULT_VHOST
> RabbitMQ virtual host. Defaults to `my_vhost`.

RABBITMQ_NODE_PORT
> RabbitMQ service port number. Defautls to `5672`

The following variables are set in defaults/main.yml and can be overriden at execution time:

The same variables are also available in defaults for standalone container execution.

Dependencies
------------

None

Example run
----------------

Run the following commands to install the service

```
# Set the working directory to your Ansible Container project root
$ cd myproject

# Install the service
$ ansible-container install bingoarun.rabbitmq-container-role
```

License
-------

MIT

Author Information
------------------

Arun prasath - [@bingoarun](https://github.com/bingoarun)
