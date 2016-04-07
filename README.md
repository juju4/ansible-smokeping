[![Build Status](https://travis-ci.org/juju4/ansible-smokeping.svg?branch=master)](https://travis-ci.org/juju4/ansible-smokeping)
# Smokeping ansible role

A simple ansible role to setup smokeping
http://oss.oetiker.ch/smokeping/

## Requirements & Dependencies

### Ansible
It was tested on the following versions:
 * 1.9
 * 2.0

### Operating systems

Tested with vagrant on Ubuntu 14.04, Kitchen test too.
Build for Debian/Ubuntu currently with apache2.

## Example Playbook

Just include this role in your list.
For example

```
- host: all
  roles:
    - smokeping
```

After installation, connect on https://SERVER/smokeping/smokeping.cgi
and update Targets/Probes

## Variables

Nothing specific for now.

## Continuous integration

This role has a travis basic test (for github), more advanced with kitchen and also a Vagrantfile (test/vagrant).

Once you ensured all necessary roles are present, You can test with:
```
$ cd /path/to/roles/smokeping
$ kitchen verify
$ kitchen login
```
or
```
$ cd /path/to/roles/smokeping/test/vagrant
$ vagrant up
$ vagrant ssh
```

## Troubleshooting & Known issues


## License

BSD 2-clause

