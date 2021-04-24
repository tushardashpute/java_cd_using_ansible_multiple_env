# java_cd_using_ansible_multiple_env
java_cd_using_ansible_multiple_env

To clone the git repo:

git clone https://github.com/cloudtechmasters/springboohello-CICD.git

Add the host entry for different env in inventory file at default (/etc/ansible/inventory) or we can use custom location as well.
If we are using custom location need to pass it as "ansbile-plabook playbook.yml -i inventory_file"

How we can run it:

ansible-playbook helloworld_setup.yml --extra-vars '{"target_hosts":"dev"}' --extra-vars '{"version":"0.1.0"}'

ansible-playbook helloworld_setup.yml --extra-vars '{"target_hosts":"dev"}' --extra-vars '{"version":"0.2.0"}'

ansible-playbook helloworld_setup.yml --extra-vars '{"target_hosts":"prod"}' --extra-vars '{"version":"0.1.0"}'

