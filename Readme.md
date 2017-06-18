
# Install Ansible

## CentOS 7

```
centos:~ # yum install epel-release
centos:~ # yum makecache
centos:~ # yum install ansible
```

## Debian 8

```
debian:~ # vi /etc/apt/sources.list
deb http://ppa.launchpad.net/ansible/ansible/ubuntu trusty main

debian:~ # apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 93C4A3FD7BB9C367
debian:~ # apt-get update
debian:~ # apt-get install ansible
```

## Ubuntu 16

```
ubuntu:~ $ sudo apt-get install software-properties-common
ubuntu:~ $ sudo apt-add-repository ppa:ansible/ansible
ubuntu:~ $ sudo apt-get update
ubuntu:~ $ sudo apt-get install
```

---


# Run Playbook

```
linux:~ # ansible-play site.yml -v

# for RHEL
rhel:~ # ansible-playbook site.yml -v -e 'repo_url=file:///mnt'

# for SLES
sles:~ # ansible-playbook site.yml -v -e 'repo_url=cd:///?devices=/dev/disk/by-id/ata-VBOX_CD-ROM'
```

