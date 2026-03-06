# Basic-Server-Setup-Task-4

## Project Description
This project demonstrates how to configure a basic local web server on a Linux virtual machine using Apache. The Apache web server was installed on Ubuntu, configured, and used to host a simple HTML webpage. The project shows how a web server can serve content from the web root directory (/var/www/html) and be accessed locally through a web browser.

## Technologies Used
* Ubuntu Linux
* Apache Web Server
* HTML
* Hyper-V Virtual Machine

## 1. Server Installation
First, the system package list is updated:

sudo apt update

Then the Apache web server was installed;

sudo apt install apache2 -y

<img width="1009" height="434" alt="image" src="https://github.com/user-attachments/assets/163a016f-e0ed-4c67-9355-6118763ff5b4" />


## 2. Starting the Apache Service
After installation, the Apache service was started and verified using;

sudo systemctl status apache2

This confirms that the web server is running properly.

<img width="1027" height="711" alt="image" src="https://github.com/user-attachments/assets/7fa56fdb-5687-4853-8417-8917cf22b931" />


## 3. Web Root Directory
Apache stores website files in the following directory:

index.html

<img width="1017" height="781" alt="image" src="https://github.com/user-attachments/assets/31891c89-37bc-4645-95e2-5a42b644a99b" />


## 4. Folder Structure
/var/www

└── html

 └── index.html

<img width="1011" height="771" alt="image" src="https://github.com/user-attachments/assets/77833ca2-b156-4d0e-9810-e5fab17c7e4b" />


## 5. Creating a Custom Webpage
The default Apache webpage was replaced with a custom HTML using using:

sudo nano /var/www/html/index.html

<img width="1022" height="772" alt="image" src="https://github.com/user-attachments/assets/3a55350f-5500-476f-b098-04530b55529f" />



## 6. Testing the Web server
The web server was tested by opening a browser and navigating to: 

http://localhost

This successfully displayed the custom webpage, confirming that the server is hosting web content correctly.

<img width="1024" height="777" alt="image" src="https://github.com/user-attachments/assets/4ea940d7-96f7-4cca-976c-03ff1cff9ac7" />


## Learning Outcome
Throughout this project I learned how to:
* Install and configure a web server on Linux
* Manage services using systemctl
* Understand the web root directory
* DEploy a basic webpage on a local server
