
```
sudo yum update -y

sudo yum install -y python-pip python-devel git && sudo yum group install -y "Development Tools" && sudo reboot

git clone https://github.com/thatcoderguy/openshift-3.11-CentOS-9
cd openshift-ansible

sudo pip install -r requirements.txt
sudo pip install pyopenssl --upgrade

sudo cp -r /usr/local/bin/* /usr/bin

sudo yum install https://rpmfind.net/linux/centos-stream/9-stream/BaseOS/x86_64/os/Packages/openssl-libs-3.2.1-1.el9.i686.rpm

sudo ansible-playbook -i inventory/hosts.localhost playbooks/prerequisites.yml
sudo ansible-playbook -i inventory/hosts.localhost playbooks/deploy_cluster.yml

```

