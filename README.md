
```
sudo yum update -y

sudo yum install -y python-pip python-devel git && sudo yum group install -y "Development Tools" && sudo reboot

git clone https://github.com/thatcoderguy/openshift-3.11-CentOS-9
cd openshift-ansible

sudo pip install -r requirements.txt
sudo pip install pyopenssl --upgrade

sudo cp -r /usr/local/bin/* /usr/bin

sudo yum install https://rpmfind.net/linux/centos-stream/9-stream/BaseOS/x86_64/os/Packages/openssl-libs-3.2.1-1.el9.i686.rpm

sudo yum install https://rpmfind.net/linux/opensuse/distribution/leap/15.6/repo/oss/x86_64/libopenssl10-1.0.2p-150000.3.91.1.x86_64.rpm

sudo yum install https://rpmfind.net/linux/atrpms/el5-x86_64/atrpms/stable/libpth20-2.0.7-6.0.el5.x86_64.rpm
sudo yum install https://rpmfind.net/linux/dag/redhat/el5/en/x86_64/dag/RPMS/gpgme-1.1.8-1.el5.rf.x86_64.rpm
sudo yum install https://rpmfind.net/linux/atrpms/el5-x86_64/atrpms/stable/libgpgme-pthread11-1.1.6-22.el5.x86_64.rpm

#sudo yum install https://rpmfind.net/linux/centos-stream/9-stream/BaseOS/x86_64/os/Packages/python3-gpg-1.15.1-5.el9.x86_64.rpm
#sudo yum install https://rpmfind.net/linux/centos-stream/9-stream/BaseOS/x86_64/os/Packages/python3-3.9.19-8.el9.x86_64.rpm



sudo yum install https://rpmfind.net/linux/openmandriva/5.0/repository/x86_64/main/release/python-pyyaml-6.0-2-omv4090.x86_64.rpm
sudo yum install https://rpmfind.net/linux/openmandriva/5.0/repository/x86_64/main/release/python-slip-0.6.5-4-omv4090.noarch.rpm
sudo yum install https://rpmfind.net/linux/openmandriva/5.0/repository/aarch64/main/release/python-slip-dbus-0.6.5-4-omv4090.noarch.rpm

#sudo yum install https://rpmfind.net/linux/fedora/linux/releases/39/Everything/x86_64/os/Packages/g/glibc-all-langpacks-2.38-7.fc39.x86_64.rpm
#sudo yum install https://rpmfind.net/linux/fedora/linux/releases/39/Everything/x86_64/os/Packages/g/glibc-2.38-7.fc39.x86_64.rpm
#sudo yum install https://rpmfind.net/linux/fedora/linux/releases/39/Everything/x86_64/os/Packages/g/glibc-common-2.38-7.fc39.x86_64.rpm
#sudo yum install https://rpmfind.net/linux/fedora/linux/releases/39/Everything/x86_64/os/Packages/g/glibc-2.38-7.fc39.i686.rpm



sudo yum install https://rpmfind.net/linux/opensuse/tumbleweed/repo/oss/x86_64/libpython2_7-1_0-2.7.18-49.1.x86_64.rpm

sudo yum install https://rpmfind.net/linux/openmandriva/5.0/repository/x86_64/main/release/python2-2.7.18-5-omv2390.x86_64.rpm

sudo yum install https://kojipkgs.fedoraproject.org//vol/fedora_koji_archive01/packages/python-ipaddress/1.0.7/3.fc22/noarch/python-ipaddress-1.0.7-3.fc22.noarch.rpm

sudo yum install https://www.python.org/ftp/python/2.3/rpms/redhat-9/python2.3-2.3-5pydotorg.i386.rpm  **enable /etc/yum.repo.d/rpmfinder.repo first
sudo yum install https://rpmfind.net/linux/atrpms/sl4-x86_64/atrpms/stable/pythonabi-2.3-3.el4.at.x86_64.rpm
sudo yum install https://rpmfind.net/linux/atrpms/el4-x86_64/atrpms/stable/rpm-python-4.4.2-15.2_60.el4.at.x86_64.rpm

sudo ansible-playbook -i inventory/hosts.localhost playbooks/prerequisites.yml
sudo ansible-playbook -i inventory/hosts.localhost playbooks/deploy_cluster.yml

```

