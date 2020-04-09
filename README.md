ansible-role-local-private-public-keys
=========

When you want to connect to the Ansible controller machine, remotely from another machine, you need to have a pair of public/private keys configured to a user who can access and run Ansible playbooks.
This role creates a pair of private/public keys and optionally adds the public key to the `authorized_key` file. Then you can take the private key and use it in another machine. For me, I use it in Gitlab, to call my Ansible controller node and run deployment playbooks.

Requirements
------------

None

Role Variables
--------------

Check the file [defaults/main.yml](./defaults/main.yml) for details.

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

MIT

Author Information
------------------

Milad Kawas. @miladkawas
