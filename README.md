## Use to deploy the app with command line

export HISTCONTROL=ignorespace:ignoredups
ansible-playbook deploy_nodejs_app.yml -i "ubuntu1@192.168.1.114," -e "ansible_hosts=all" -e "repo_url=https://github.com/ndemeyvan/ansible_react.git" -e "container_name=<container_name>" -e "docker_image_name=<image_name>" -e "ansible_become_password='<user_machine_password>'"
history -d $((HISTCMD-1))
