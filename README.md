test task ansible playbooks
===================


Clonning repo
`git clone https://github.com/knopka/test_task_ansible.git`


Installing python app. Installing and configuring Nginx.
`ansible-playbook -i 'localhost, ' -c local deploy.yml --ask-become-pass`


Installing Jenkins. There is no image with Jenkins version 1.656, so I built image based on jenkins:1.651.3 and then just deployed jenkins.war from version 1.656.
`ansible-playbook -i 'localhost, ' -c local jenkins_install.yml --ask-become-pass`


Creating Jenkins job
`ansible-playbook -i 'localhost, ' -c local jenkins_job.yml --ask-become-pass`

