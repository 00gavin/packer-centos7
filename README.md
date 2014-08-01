# A Packer build to generate a CentOS 7 Vagrant Box

This repository will generate a CentOS 7 box for Vagrant with Packer.

Getting started...

* Install VirtualBox https://www.virtualbox.org/wiki/Downloads
* Install Vagrant http://www.vagrantup.com/downloads
* Install Packer http://www.packer.io/downloads.html
* Download the CentOS 7 Minimal ISO and copy/link it into the repo directory http://isoredirect.centos.org/centos/7/isos/x86_64/

Build it...

```
$ packer build centos7.json
```

Test it out...

```
$ vagrant up
$ vagrant ssh
```

