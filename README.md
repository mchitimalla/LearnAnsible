# LearnAnsible
ansible --version
ansible -i /tmp/inv all -e ansible_user=centos -e ansible_password=DevOps321 -m ansible.builtin.ping
rm -rf .ansible/ ------Remove Cache
ansible -i /tmp/inv all -e ansible_user=centos -e ansible_password=DevOps321 -m ansible.builtin.yum -a name=nginx

ansible-playbook -i /tmp/inv -e ansible_user=centos -e ansible_password=DevOps321 LearnAnsible/print.yml
ansible-pull localhost, -U  https://github.com/mchitimalla/LearnAnsible.git print.yml
# In Ansible variable will be accessed using {{ }} ,
# Ansible Supports double quotes and single quotes also , However quotes are not not mandatory in all cases
# quotes are mandatory if value starts with a variable , meaning
# msg: {{ URL }} <- This requires quoting
# msg: URL - {{ URL }} <- This does not require quoting
