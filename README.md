# sshkey_management
managing the general ssh key automation using ansible 

# PlayBook prerequisites 

1 -> Change the host file accordin to your needs i have used generalised ip address

2 -> To excute this playbook you need to install python passlib module as i'm using "vars_prompt:" 

# Execting the playbook 

* In this play book i have used tags so you can execute the tasks againts tags. 

* To list tags in play book 
  * ansible-playbook  -vvv main.yml --list-tags
  * you can ignore -vvv if dont want to see the verbose ouput
  
* To execute the play with tags 
  * ansible-playbook main.yml --tags generate_ssh_keys

* List of tags in the play book 
  * add_new_users
  * generate_ssh_keys
  * copy_public_key
  * deleting_users

* When you execute the playbook it will prompt for 
  * hostname 
  * Username

