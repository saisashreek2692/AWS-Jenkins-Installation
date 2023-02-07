# AWS-Jenkins-Installation
This repo gives commands for jenkins installation in AWS EC2 Instance.

## To Install Jenkins on AWS EC2 Instance

Step 1: Login to your AWS Console

Step 2: Go to EC2 Instance Service

Step 3: Create or Launch EC2 Service

Step 4: Connect EC2 Service in Windows / Mac / Linux

Step 4.1: To connect EC2 Instance in Windows using CMD / Powershell Method.

Step 4.1.1: Download newly created Key pair for your instance in .pem file and save it in safe folder. 

Step 4.1.2: Open Command Promt / Powershell in Windows as Administrative, then type ```ssh```.

Step 4.1.3: Now copy EC2 Instance IP Address from AWS Console.

Step 4.1.4: Type, ``` ssh -i /path/key-pair-name.pem instance-user-name@instance-public-dns-name ```

Step 4.1.5: In Command Prompt, after succesfully connected to EC2 Instance, we could able to see our selected OS Image on screen.

Step 4.1.6: Type, ``` sudo su ```. Follow the steps from here on.

Step 4.1.7: Navigate to Jenkins website, use this link: ``` https://pkg.jenkins.io/redhat-stable/ ```. This link will help us to download proper Jenkins file on our EC2 Instance.

Step 4.1.8: ``` sudo wget -O /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo ```.

Step 4.1.9: ``` sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io.key  ```.

Step 4.1.10: ``` yum install fontconfig java-11-openjdk -y ```.

Step 4.1.11: ``` yum install jenkins -y ```.

Step 4.1.12: After following the above steps, now check your Jenkins. ``` jenkins --version ```.

Step 4.1.13: If you can see Jenkins version this installation is succesful.

Step 4.1.14: Now goto, EC2 Instance Security Group, Select Inbound rule && Edit rule.

Step 4.1.15: ``` All Traffic ```, ``` Any where IP ```, ``` Save ```.
