# Api Automation Testing With Jenkins

## Technology and Tool Used
- Postman
- Node Js
- Newman
- Jenkins
- npm
- Visual Studio Code

## Prerequisites

- You must have installed node js to your system
- Postman
- NPM
- Newman
- Jenkins

## Scenario of this project

- User Can't Login With Invalid Email
- User Can't Login With Invalid Password
- User Can't Login With Valid Email And Invalid Password
- User Can't Login With  Invalid Email And Valid Password
- User Can Login With Valid Credential
- Can't Create a User With Invalid Token
- Can't Create a User With Invalid SECRET-KEY
- Can't Create a User With Invalid Token And Valid  SECRET-KEY
- Can't Create a User With Invalid SECRET-KEY And Valid Token
- Create User With Valid Credential
- Can't get user list  With Invalid Token
- User can't search with wrong user id
- User can get user list with valid credential
- User can search user by user id
- Can't Update User With Invalid SECRET-KEY
- User can update a user with valid credential
- Can't Delete User  With Invalid Token
- Can't Delete User  With Invalid SECRET-KEY
- User can delete a user with valid credential
- Can't Create  Agent With Invalid Token
- Can't Create a Agent With Invalid SECRET-KEY
- Can't Create Agent With Invalid Token And Valid  SECRET-KEY
- Can't Create Agent With Invalid SECRET-KEY And Valid Token
- Create Agent With Valid Credential

## API Documents



      https://documenter.getpostman.com/view/16548351/2s9YeD8t6m

## How to run this project

- clone this project
- open this project in Visual Studio code

## npm install

             npm install
            
- check the npm version

         npm -v
  
## Newman Install

      npm install -g newman
  
- check the newman version

    newman -v
  
## Jenkins Install

### Prerequisites

- Minimum hardware requirements:

- 256 MB of RAM

- 1 GB of drive space (although 10 GB is a recommended minimum if running Jenkins as a Docker container)

- Recommended hardware configuration for a small team:

- 4 GB+ of RAM

- 50 GB+ of drive space

### Comprehensive hardware recommendations:

- Hardware: see the Hardware Recommendations page

### Software requirements:

- Java: see the Java Requirements page

- Web browser: see the Web Browser Compatibility page

- For Windows operating system: Windows Support Policy

- For Linux operating system: Linux Support Policy

- For servlet containers: Servlet Container Support Policy

## Installation steps using Windows MSI installer

- Refer to the Windows section of the Downloading Jenkins page to download either an LTS release or a weekly release of the Windows installer.
  After the download completes, open the Windows installer and follow the steps below to install Jenkins.
  
### Step 1: Setup wizard
On opening the Windows Installer, an Installation Setup Wizard appears, Click Next on the Setup Wizard to start your installation.

![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/3293d6be-729c-4cdf-9405-761e01f066b7)

### Step 2: Select destination folder

Select the destination folder to store your Jenkins Installation and click Next to continue.

![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/84142c16-945c-42c4-86ac-2cbbb5576c8b)


### Step 3: Service logon credentials

When Installing Jenkins, it is recommended to install and run Jenkins as an independent windows service using a local or domain user as it is much safer than running Jenkins using LocalSystem(Windows equivalent of root) which will grant Jenkins full access to your machine and services.

To run Jenkins service using a local or domain user, specify the domain user name and password with which you want to run Jenkins, click on Test Credentials to test your domain credentials and click on Next.

Jenkins Service Logon Credentials

If you get Invalid Logon Error pop-up while trying to test your credentials, follow the steps explained here to resolve it.

![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/26a7cbd6-1457-40ee-9c84-4d2a615ce55d)


### Step 4: Port selection

Specify the port on which Jenkins will be running, Test Port button to validate whether the specified port if free on your machine or not. Consequently, if the port is free, it will show a green tick mark as shown below, then click on Next.

![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/15a9cfd8-1afb-44aa-b52d-2e3e3100218d)

### Step 5: Select Java home directory

The installation process checks for Java on your machine and prefills the dialog with the Java home directory. If the needed Java version is not installed on your machine, you will be prompted to install it.

Once your Java home directory has been selected, click on Next to continue.

Select Java Home Directory

![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/946b1319-9327-4563-9cb5-54c37999d158)


### Step 6: Custom setup

Select other services that need to be installed with Jenkins and click on Next.


![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/277dffef-360e-4467-aca6-1d209462daa3)


### Step 7: Install Jenkins

Click on the Install button to start the installation of Jenkins.

Additionally, clicking on the Install button will show the progress bar of installation, as shown below:

Windows Installation Progress


![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/03da8811-ee5b-46cb-b4a0-ec8437beb092)


#### Step 8: Finish Jenkins installation

Once the installation completes, click on Finish to complete the installation.


![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/3c681ad4-0892-4874-986d-510bf46a21b2)


Jenkins will be installed as a Windows Service. You can validate this by browsing the services section, as shown below:

![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/679c8971-df0e-4c6c-8de2-bfd239ff1f0a)


## Post-installation setup wizard

- When you first access a new Jenkins instance, you are asked to unlock it using an automatically-generated password.

### Step 1

Browse to http://localhost:8080 (or whichever port you configured for Jenkins when installing it) and wait until the Unlock Jenkins page appears.

![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/e1d25c71-ff6f-44b5-9d33-5e376b333a77)

## Step 2

- The initial Administrator password should be found under the Jenkins installation path (set at Step 2 in Jenkins Installation).

- For default installation location to C:\Program Files\Jenkins, a file called initialAdminPassword can be found under C:\Program Files\Jenkins\secrets.

However, If a custom path for Jenkins installation was selected, then you should check that location for initialAdminPassword file.
- 
![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/40b287b3-8fe2-4d2e-9c92-b7fa573679af)


## Step 3

- Open the highlighted file and copy the content of the initialAdminPassword file.

![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/b2a955c5-6725-46cd-a005-287be03faa42)

## Step 4

- On the Unlock Jenkins page, paste this password into the Administrator password field and click Continue.
- Notes:

- You can also access Jenkins logs in the jenkins.err.log file in your Jenkins directory specified during the installation.

- The Jenkins log file is another location (in the Jenkins home directory) where the initial password can also be obtained.

![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/e46a7185-0e4f-410c-9085-486c00ff97ac)

## After Installation 

          npm install -g newman-reporter-htmlextra

          newman run collection.json -r htmlextra

          
- then create a new item in Jenkins and configure

![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/5185b45b-8b1b-4fa4-8782-a02a7de12189)

![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/718b74ca-5b54-44ee-8303-a3a40800b3d3)

![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/2e7d1b8e-cdd2-4890-a92f-404c85d76b09)

 
- After configuring then build this item
- then automatically create a newman html extra report in the right directory

 ### Output: 

![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/2c6598ce-89ab-41e3-ad9f-77fe42fdb27b)

![image](https://github.com/Mamun104/newman-reporter-htmlextra-with-jenkins/assets/78067017/a18b1192-baa0-46ab-8e87-67f420952144)

