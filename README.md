charm-bootstrap-ansible
=======================

A quick way to get started creating a juju charm using
ansible:

```
$ mkdir -p jujulocalrepo/precise && cd jujulocalrepo/precise
$ git clone https://github.com/absoludity/charm-bootstrap-ansible.git mycharm
$ cd mycharm
$ make
```

That will pull in the required charm-helpers library and run the unit-tests.
Take a look around at the hooks/hooks.py or the playbooks/site.yaml,
or deploy it with:

```
$ juju deploy --repository=../.. local:charm-bootstrap-ansible
```

TODO:
-----
 * Add metadata and test deploy
 * Add template with example in configur hook.
 * Update playbook to demo common things (ie. code on server etc.)

[1]: http://ansibleworks.com/
