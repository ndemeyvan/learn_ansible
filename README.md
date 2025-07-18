## Use to deploy the app with command line

export HISTCONTROL=ignorespace:ignoredups
 ansible-playbook deploy_react_container.yml -i "ubuntu1@192.168.1.114," -e "ansible_hosts=all" -e "repo_url=https://github.com/ndemeyvan/ansible_react.git" -e "container_name=flexy_push_6" -e "docker_image_name=flexy_push_6" -e "ansible_become_password='  '"
history -d $((HISTCMD-1))

