## Damn Vulnerable Web App Vagrant environment
[Damn Vulnerable Web App](https://github.com/RandomStorm/DVWA) vagrant things. Should make bootstrapping a new instance for testing much easier..

### requirements
- vagrant w/ Virtualbox guest additions
- ubuntu14.04 vagrant box

```
$ git clone https://github.com/dustyfresh/vagrant-dvwa.git
$ cd vagrant-dvwa && vagrant up
# be sure to run in bridged mode
$ vagrant ssh
vagrant@dvwa:~$ ip a
```
