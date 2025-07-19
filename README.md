## Use to deploy the app with command line

export HISTCONTROL=ignorespace:ignoredups
 ansible-playbook deploy_nodejs_app.yml -i "ubuntu1@192.168.1.114," -e "ansible_hosts=all" -e "repo_url=https://github.com/ndemeyvan/ansible_nestjs.git" -e "container_name=flexy_push_12" -e "docker_image_name=flexy_push_12" -e "ansible_become_password='  '" -e "app_type='nestjs'" -e "node_version='22-alpine'"
history -d $((HISTCMD-1))
