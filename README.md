# Bosch-Round-2
This repository hosts BOSCH CONNECTED INDUSTRY PROGRAMING CHALLENGE codebase


The app folder contains the todo app sorce code and docker-compose file


The **main.yml** is the ansible deployment playbook.


When the main.yml is executed, it invokes **3 roles** from the roles directory :
1st role (**docker_installation**) will install Docker and prerequisites,
2nd role (**copy_app_files**) will copy the the todo app source files to the target machine (ubuntu)
3rd role (**docker-compose**) will invoke the docker-compose file when called in the main.yml 

The ansible inventory is present at **ansible_hosts** file


The pem key **anand.pem** is used for connecting to the ubuntu machine (hosted in AWS) (machine username: ubuntu)


The ansible configuration settings are defined in **ansible_cfg** file


The output of this assignment can be viewed from this **publicip:port 54.165.146.231:3000**





