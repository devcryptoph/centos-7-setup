# Centos-7-Setup HOWTO

### Update and Install RPM dependencies

`yum check-update`

`yum -y update` 

`yum install git ansible`

`reboot`



#### clone repository

`git clone https://github.com/devcryptoph/centos-7-setup.git`

`cd centos-7-setup`

`ansible-playbook -i inventory -vvv main.yml` 

