riakcs-credentials
==================

A brief description of the role goes here.

Requirements
------------

- requests

Role Variables
--------------

| Name | Default | Description
|--- |--- |---
| json_file_path | /tmp | Folder in which will be stored the created credentials
| user_name | admin | Username of the credentials
| user_mail | admin@riak | User's mail address


Dependencies
------------

If you don't have your RiakCS cluster already, using riakcs-cluster role will have it created for you.

- JohnPreston.riakcs-cluster

Example Playbook
----------------

```

- hosts: riakcs_nodes
  roles:
  - JohnPreston.riakcs-credentials

```

```

- hosts: riakcs_nodes
  roles:
  - JohnPreston.riakcs-credentials
  - json_file_path: /root/
  - user_name: john
  - user_mail: john@ews

```


License
-------

None

Author Information
------------------

John Preston [John Mille]

