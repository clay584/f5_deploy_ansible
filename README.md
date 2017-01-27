# f5_deploy_ansible
Deploy F5 devices with Ansible

## Installation

	sudo yum install ansible -y
    sudo pip install bigsuds f5-sdk
    git clone https://github.com/clay584/f5_deploy_ansible.git
    cd /tmp
    git clone https://github.com/F5Networks/f5-ansible.git
    mv /tmp/f5-ansible/library/* ~/f5_deploy_ansible/library/
    rm -rf /tmp/f5-ansible
    cd ~/f5_deploy_ansible

## Usage

First, update the f5_deploy_ansible/hosts file to inlcude all of the devices that you want to configure.  Then run...

    ansible-playbook -i inventory.yml site.yml
