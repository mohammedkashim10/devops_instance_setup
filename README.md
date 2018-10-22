# Amazon Web Services (AWS) Instance Setup
1. Select 'Services' from the Navbar
2. Select 'EC2' from the options
3. Under the 'Create Instance' header, click 'Launch Instance'
	* Step 1: Choose AMI; select the machine with your desired operating system
	* Step 2: Choose an Instance Type; select the desires instance and click 'Next'
	* Step 3: Configure Instance Details; leave as default settings and click 'Next'
	* Step 4: Add Storage; leave as default settings and click 'Next'
	* Step 5: Add Tags; add any desired tags as key value pairs and click 'Next'
	* Step 6: Configure Security Group; add security groups for different ports as desired and click 'Review and Launch'
	* Step 7: Review Instance Launch; check to see if everything is to your liking and click 'Launch' if so
4. Copy your pem file into your .ssh directory
5. Change the permissions using ```chmod 400 ~/.ssh/DevOpsStudents.pem```
(in this example, the file is called DevOpsStudents.pem)

6. Spin up the machine using by running
```ssh -i ~/.ssh/DevOpsStudents.pem ubuntu@*Public DNS*```
where the Public DNS can be found on AWS