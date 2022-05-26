# DevOps-project11

# Step 1: Install and configure Ansible
-  I updated the name of the  Jenkins server to Jenkins-ansible
- Created a new reposistory named "ansible-config-mgt" 
- Installed Ansible using the following commands
    ```
    sudo apt update
    sudo apt install ansible
    ansible --version
    ```
   ![alt text](https://github.com/Ellawangari/DevOps-Project11/blob/main/imgs/1.PNG)
   ![alt text](https://github.com/Ellawangari/DevOps-Project11/blob/main/imgs/2.PNG)
   
- ## Configure Jenkins build job to save artifacts after every change.
  - Created a Freestyle project named ansible and pointed it to the ansible-config-mgt repo
  - Configured webhook in GitHub and set the webhook to trigger ansible build.
  - Configured a post-build job to archive the artifacts
     ![alt text](https://github.com/Ellawangari/DevOps-Project11/blob/main/imgs/4.PNG)
     ![alt text](https://github.com/Ellawangari/DevOps-Project11/blob/main/imgs/5.PNG)
     ![alt text](https://github.com/Ellawangari/DevOps-Project11/blob/main/imgs/6.PNG)
    ![alt text](https://github.com/Ellawangari/DevOps-Project11/blob/main/imgs/7.PNG)
    
  # Step 2: Begin Ansible development
  Created a new branch in your ansible-config-mgt repo.
  - Checked out to the newly created branch
  - Created playbooks directory for storing playbooks
  - Created an inventory directory for storing inventory files
  - In the playbooks folder, I created a common.yml file and on the inventry folder i also  created dev.yml, prod.yml, staging.yml and uat.yml for dev, prod, staging and uat for repective environments
![alt text](https://github.com/Ellawangari/DevOps-Project11/blob/main/imgs/8.PNG)
![alt text](https://github.com/Ellawangari/DevOps-Project11/blob/main/imgs/9.PNG)

  # Step 3: Set up ansible inventory, created a common playbook
  - Created the inventory file and updated it with the necessary server details
  - Copied the contents of my ssh file 
  - ![alt text](https://github.com/Ellawangari/DevOps-Project11/blob/main/imgs/10.PNG)
  - Then push the  changes of my branch
  -  ![alt text](https://github.com/Ellawangari/DevOps-Project11/blob/main/imgs/11.PNG)
  -  The jenkins automatically created a build of the commited and pushed code
  -  ![alt text](https://github.com/Ellawangari/DevOps-Project11/blob/main/imgs/12.PNG)

 # Step 4: Run Ansible
 - Use the ansible playbook command to execute the ansible playbook and inventory files
 -  ![alt text](https://github.com/Ellawangari/DevOps-Project11/blob/main/imgs/14.PNG)
   -  ![alt text](https://github.com/Ellawangari/DevOps-Project11/blob/main/imgs/16.PNG) 
   -  Then went a head to onfirm that wireshark was succesfully installed.
   -  ![alt text](https://github.com/Ellawangari/DevOps-Project11/blob/main/imgs/n.PNG) 


  
