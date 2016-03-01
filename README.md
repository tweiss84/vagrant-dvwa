## Damn Vulnerable Web App Vagrant environment
### requirements
- vagrant w/ Virtualbox guest additions
- ubuntu14.04

```
$ git clone https://github.com/dustyfresh/vagrant-dvwa.git
$ cd vagrant-dvwa && vagrant up
# be sure to run in bridged mode
$ vagrant ssh
vagrant@dvwa:~$ ip a
```
