# LS3 OpenStack Admin API

## Introduction

This repository contains some customized scripts to access the LS3 OpenStack cloud. The scripts are based on the the [OpenStack command line client](http://docs.openstack.org/developer/python-openstackclient/).

## Requirements and Installation

The scripts require Python and some additional libraries. It is recommend to run Python in a [virtual environment](https://virtualenv.pypa.io/). Run the following commands in a Linux shell (tested on Debian Jessy 64-bit) to install the whole environment including the customized scripts itself.

```
sudo apt-get update
sudo apt-get install -y git
sudo apt-get install -y jq
sudo apt-get install -y python-dev python-pip
sudo pip install virtualenv
git clone https://github.com/lsinfo3/openstack-admin.git
cd openstack-admin
virtualenv venv
source venv/bin/activate
pip install -r requirements.txt
```

Usage:
```
source venv/bin/activate
source os-auth
os-project-create
```
