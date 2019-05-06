# axelerant_technical

Code is written in Ansible. The main file can be found in ./roles/grant_revoke/tasks/main.yml.
"Access permissions" and the "user" are taken as variable to ansible script. Below are the steps to run the code

## Steps to run the code
1. Make sure Ansible is installed in the system. Installation instructions can be found here, [ansible_install](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html#latest-releases-via-pip)
2. Clone the repository as below

   `git clone https://github.com/adityacs/axelerant_technical.git`
3. Change direcotry

   `cd axelerant_technical`
4. If you have real servers to test you can change the IP address and hostname in iventory.ini file.
5. Then run below command to provide access to a user

   `ansible-playbook -i inventory.ini playbooks/grant_revoke.yml -e access=grant -e user=aditya`
6. To revoke access to a user you can run below command

   `ansible-playbook -i inventory.ini playbooks/grant_revoke.yml -e access=revoke -e user=aditya`
   
   
## Note

Please email me at aditya.gnu@gmail.com if you have any questions.
