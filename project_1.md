# PROJECT 1 DOCUMENTATION: LAMP STACK IMPLEMENTATION

Scope: to gain familiarity with the Linux terminal and commands,  to generate and implement LAMP components 

## Step 1: Setting up OpenSSH server and connecting to EC2 instance

 

Links used for help 
 [Install OpenSSH for Windows](https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse?tabs=powershell)             [Key-based authentication in OpenSSH for Windows](https://learn.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement)

![connecting to e2c instance](./images/conncet_ec2_instance1.png)

## Step 2: Installing Apache and updating the Firewall


![sudo apt install apache2](./images/sudo_apt_install_apache2.png)


## Step 3: Installing MySQL


![mysql installation](./images/installing_mysql.png)


### Setting password for root user on MySQL

- Running `sudo mysql_secure_installation`  for password validation

At this point, I had trouble figuring out how to enter the password, as nothing appeared on my screen as I typed. Later, I realized I wasn't supposed to see the password while typing. I was able to set a new password for the root user.

![password](./images/setting_password_mysql_2.png)

## Step 4: Installing PHP

Installed PHP components using `sudo apt install php libapache2-mod-php php-mysql`

 PHP version was confirmed with `php -v`

![php version](./images/php_version.png)

## **Step 5: Creating Virtual Host with Apache**

- Directory created for Apache was named *projectlamp*
 
    `sudo mkdir /var/www/projectlamp` 
- The Virtual Host for Apache was successful in returning message to index.html file

![testing virtual host](./images/testing_website.png)

## **Step 6: enabling PHP on the website**

When my reload of Apache failed, I looked up the error on Google and found that it was caused by a syntax error. Using `apache2ctl configtest`, I found that the error was in dir.conf, which I had recently modified. After deleting the error I was able to succsessfully reload the Apache.

![error](./images/apache2_reload_error.png)

![php install](./images/PHP_test_script.png)
 















