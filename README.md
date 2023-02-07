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
