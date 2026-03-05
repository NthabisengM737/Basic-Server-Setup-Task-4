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

(screenshot)

## 2. Starting the Apache Service
After installation, the Apache service was started and verified using;

sudo systemctl status apache2

This confirms that the web server is running properly.

(screenshot)

## 3. Web Root Directory
Apache stores website files in the following directory:

index.html

(screenshot)

## 4. Folder Structure
/var

└── www

      └── html

        └── index.html

(screenshot)

## 5. Creating a Custom Webpage
The default Apache webpage was replaced with a custom HTML using using:

sudo nano /var/www/html/index.html

(screenshot)

## 6. Testing the Web server
The web server was tested by opening a browser and navigating to: 

http://localhost

This successfully displayed the custom webpage, confirming that the server is hosting web content correctly.

(screenshot)

## Learning Outcome
Throughout this project I learned how to:
* Install and configure a web server on Linux
* Manage services using systemctl
* Understand the web root directory
* DEploy a basic webpage on a local server
