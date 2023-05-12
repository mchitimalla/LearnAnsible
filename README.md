# LearnAnsible
ansible --version
ansible -i /tmp/inv all -e ansible_user=centos -e ansible_password=DevOps321 -m ansible.builtin.ping
rm -rf .ansible/ ------Remove Cache
ansible -i /tmp/inv all -e ansible_user=centos -e ansible_password=DevOps321 -m ansible.builtin.yum -a name=nginx

ansible-playbook -i /tmp/inv -e ansible_user=centos -e ansible_password=DevOps321 LearnAnsible/print.yml
ansible-pull localhost, -U  https://github.com/mchitimalla/LearnAnsible.git print.yml

