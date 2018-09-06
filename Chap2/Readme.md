[all:vars]
ansible_user=vagrant
ansible_ssh_private_key_file=./.vagrant/machines/default/virtualbox/private_key

* ping
ansible -i hosts webservers -m ping

* Run playbook
ansible-playbook -i hosts web-notls.yml
ansible-playbook -i hosts web-tls.yml
