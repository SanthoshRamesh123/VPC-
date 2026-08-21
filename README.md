# EX 4 :DEPLOYMENT AND CONFIGURATION OF A PRIVATE CLOUD IN AWS
### NAME: SANTHOSH R
### REG NO: 212224230249

## Aim
To create an Amazon Virtual Private Cloud (VPC) with public and private subnets, configure a security group, and launch an EC2 instance hosting a web server within the VPC. 

## Objectives
- Create an Amazon VPC.
- Create public and private subnets.
- Configure a security group for HTTP access.
- Launch an EC2 instance inside the VPC.
- Deploy and access a web server running on the EC2 instance.



# Procedure

## Task 1: Create a Virtual Private Cloud (VPC)

1. Log in to the AWS Management Console and open the **VPC** service.
2. Select **Create VPC** and choose **VPC and More**.
3. Configure the VPC with the required CIDR block, public subnet, private subnet, Internet Gateway, and NAT Gateway.
4. Create the VPC and verify that all resources are created successfully.



## Task 2: Create Additional Subnets

1. Create a second public subnet in another Availability Zone.
2. Create a second private subnet in the same Availability Zone.
3. Associate the private route table with the new private subnet.
4. Associate the public route table with the new public subnet.
5. Verify the subnet associations.


## Task 3: Create a Security Group

1. Navigate to **Security Groups** in the VPC console.
2. Create a new security group named **Web Security Group**.
3. Add an inbound rule allowing **HTTP (Port 80)** traffic from **Anywhere (IPv4)**.
4. Save the security group.


## Task 4: Launch an EC2 Web Server

1. Open the **EC2** service and launch a new instance.
2. Select **Amazon Linux 2023 AMI** and **t2.micro** instance type.
3. Configure the instance to use the newly created VPC, public subnet, and Web Security Group.
4. Add the provided user data script to install Apache, PHP, and the sample web application.
5. Launch the instance and wait until all status checks pass.
6. Access the web server using the Public IPv4 DNS.



# Outputs


<img width="1040" height="455" alt="image" src="https://github.com/user-attachments/assets/a0b90909-8db8-465f-9d04-79debe2150c7" />



<img width="1898" height="847" alt="image" src="https://github.com/user-attachments/assets/233742a5-fc29-468e-a6dd-9ed1ff79c8a3" />

<img width="1903" height="830" alt="image" src="https://github.com/user-attachments/assets/81463d49-7a33-4fda-9307-7c539ec5f87a" />

<img width="1892" height="841" alt="image" src="https://github.com/user-attachments/assets/06a95dad-0a5d-49ed-9743-ea5966012df6" />

<img width="1902" height="857" alt="image" src="https://github.com/user-attachments/assets/06a5ded5-f867-4a74-9fc0-bd1ddf36bed5" />


# Result

Thus, a VPC was configured, an EC2 instance was launched, and the hosted web application was accessed successfully. 
