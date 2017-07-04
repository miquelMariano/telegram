Role Name
=========

Use this role to sent a telegram message

Requirements
------------

Chat bot is required.

More info, [here](https://miquelmariano.github.io/2017/02/notificaciones-automaticas-con-telegram/)

Role Variables
--------------

Variable `text` is required.
This variable, contains the text that send it with telegram

Normally, we will pass this variable in playbook

Dependencies
------------

No dependencies

Example Playbook
----------------

```yaml
- hosts: ansible
  user: root
  tasks:
    - include: ../roles/miquelMariano.telegram/tasks/main.yml
      vars:
        text: "Test message from ansible"
```

Execute playbook
----------------

```yaml
ansible-playbook playbooks/telegram.yml -i inventory/servers
```

License
-------

BSD

Author Information
------------------

[miquelMariano.github.io](https://miquelMariano.github.io) | [Twitter](https://twitter.com/miquelMariano)