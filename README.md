# f5_deploy_ansible
Deploy F5 devices with Ansible

## Installation

	yum install ansible -y
    pip install bigsuds f5-sdk
    git clone https://github.com/clay584/f5_deploy_ansible.git
    cd f5_deploy_ansible
    git clone https://github.com/F5Networks/f5-ansible.git
    mv f5-ansible/library/* library/
    rm -rf f5-ansible

## Usage

First, update your ./hosts file to inlcude all of the devices that you want to configure.  Then run...
    ansible-playbook -i inventory.yml site.yml