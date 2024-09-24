
```
sudo yum update -y

sudo yum install -y epel-release && sudo yum install -y python-pip python-devel git && sudo yum group install -y "Development Tools" && sudo reboot

git clone https://github.com/thatcoderguy/openshift-3.11-CentOS-9
cd openshift-ansible

sudo pip install -r requirements.txt
sudo pip install jinja2=2.11.3   **MIGHT NOT NEED THIS
sudo pip install pyopenssl --upgrade

sudo yum install https://rpmfind.net/linux/centos-stream/9-stream/BaseOS/x86_64/os/Packages/openssl-libs-3.2.1-1.el9.i686.rpm
sudo yum install https://rpmfind.net/linux/opensuse/distribution/leap/15.6/repo/oss/x86_64/libopenssl10-1.0.2p-150000.3.91.1.x86_64.rpm
sudo yum install https://rpmfind.net/linux/atrpms/el5-x86_64/atrpms/stable/libpth20-2.0.7-6.0.el5.x86_64.rpm
sudo yum install https://rpmfind.net/linux/dag/redhat/el5/en/x86_64/dag/RPMS/gpgme-1.1.8-1.el5.rf.x86_64.rpm
sudo yum install https://rpmfind.net/linux/atrpms/el5-x86_64/atrpms/stable/libgpgme-pthread11-1.1.6-22.el5.x86_64.rpm

sudo ansible-playbook -i inventory/hosts.localhost playbooks/prerequisites.yml
sudo ansible-playbook -i inventory/hosts.localhost playbooks/deploy_cluster.yml

```

