# ec2-ansible
An ansible playbook to deploy EC2 instance

run the following commands:

#sudo apt-get update  
#sudo apt install ansible   
#sudo apt install python3-pip  
#sudo pip3 install boto  
#ansible-vault create pass.yml  


add access and secret keys from amazon in the pass.yml:  
{
  "ec2_access_key": "Your key",   
  "ec2_secret_key": "Your key"  
}  

add this lines in ansible.cfg:  
[defaults]
host_key_checking = false
remote_user = ubuntu
private_key_file = "pem file key path"
roles_path = "roles file path"  

run the playbook with --ask-vault.   

