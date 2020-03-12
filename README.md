# docker-installation-ansible
**An explaination how to install docker using ansible playbooks in rhel7**

## order to run playbooks

1. epel.yml
2. dockermodule.yml
3. dockerinstall.yml
4. dockerstart.yml
5. dockerimage.yml

## explaination

* epel.yml will download latest epel-release to be used by ansible later to download docker
* dockermodule.yml installs all the required docker modules used by ansible (_**note**: I have downloaded docker.py as i was comfortable using python2.7 or python3 you may have to download docker-py ...check online for this kinda info_)
* dockerinstall.yml will install docker using epel-release
* dockerstart.yml will start docker daemon/service and will enable it
* dockerimage.yml will download centos:7 image, it is just for checking docker is installed properly
