
```
sudo yum update -y

sudo yum install -y epel-release && sudo yum install -y python-pip python-devel git && sudo yum group install -y "Development Tools" && sudo reboot

git clone https://github.com/thatcoderguy/openshift-3.11-CentOS-9
cd openshift-ansible

sudo pip install -r requirements.txt

--sudo pip install union

sudo ansible-playbook -i inventory/hosts.localhost playbooks/prerequisites.yml
sudo ansible-playbook -i inventory/hosts.localhost playbooks/deploy_cluster.yml

```

