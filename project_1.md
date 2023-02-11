# **PROJECT 1 DOCUMENTATION: LAMP STACK IMPLEMENTATION**

## **Running commands on terminal to connect to EC2 instance**
    1. entered directory where .pem key was saved using `cd`, in my case I typed in "cd Downloads"
    2. connected to AWS server using ssh: "ssh -i "PBL_key_pair.pem" ubuntu@ec2-13-41-225-1.eu-west-2.compute.amazonaws.com"

NOte: you need to install and configure OpenSSH server, and generate your private and public keys  

Links for help 
 [Install OpenSSH for Windows](https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse?tabs=powershell)             [Key-based authentication in OpenSSH for Windows](https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement)

![connecting to e2c instance](.\images\conncet_ec2_instance1.png)

## **Installing Apache and updating the Firewall**

Run the folliwing commanda

`sudo apt update`
    