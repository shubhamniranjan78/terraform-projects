Terraform Project: Deploying NGINX Server on AWS

This project demonstrates how to use Terraform to deploy an NGINX server on AWS with a fully automated Infrastructure as Code (IaC) approach. It includes setting up the network, configuring security, and deploying an EC2 instance.

= Features
* Create and manage AWS infrastructure using Terraform.
* Deploy an Ubuntu EC2 instance with NGINX pre-installed.
* Set up VPC, public subnet, Internet Gateway, and route tables.
* Configure security groups for HTTP (port 80) and HTTPS (port 443) traffic.
* Use terraform destroy for resource cleanup.

= Prerequisites
Before you begin, ensure you have:

- An AWS account.
- Terraform installed on your local machine (Install Terraform).
- An IAM user with appropriate permissions for provisioning AWS resources.




= Setup and Usage
1. Clone the Repository:

git clone https://github.com/shubhamniranjan78/terraform-projects.git
cd terraform-projects/project01


2. Initialize Terraform:

terraform init


3. Plan the Infrastructure:

terraform plan


4. Deploy the Infrastructure:

terraform apply

Confirm the action by typing yes when prompted.


5. Verify Deployment:

Use the public IP from the Terraform output to access the NGINX default page in a browser.


6. Clean Up Resources:

terraform destroy

Confirm the action by typing yes when prompted.



=  Configuration Files

1. providers.tf
Specifies the AWS provider and Terraform version.


2. network.tf
Defines the VPC, public subnet, Internet Gateway, and route table.


3. compute.tf
Provisions the EC2 instance and security group.


= Lessons Learned


Automating infrastructure with Terraform simplifies deployment and improves scalability.
Properly configuring security groups is essential for secure cloud environments.
Using IaC ensures consistent and repeatable infrastructure setup.
Resources
Terraform Documentation
AWS Free Tier
Contributing
Feel free to fork this repository and suggest improvements via pull requests.

License
This project is open-source and available under the MIT License.
