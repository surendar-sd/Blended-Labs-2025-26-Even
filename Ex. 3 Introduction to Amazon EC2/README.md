# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**: S.D. Surendar
* **Register Number**: 212224110052
* **Date of Submission**: 17-05-2026

---

## Objective

The objective of this experiment is to understand the fundamentals of Amazon Elastic Compute Cloud (EC2). This lab focuses on launching and managing a virtual server, understanding instance types and AMIs, connecting to an EC2 instance, monitoring its status, and performing basic instance operations such as start, stop, and terminate.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* Web browser with internet connectivity
* Basic knowledge of Linux commands (optional)

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Key Pair
* Security Group
* SSH Client (PuTTY / Terminal)

---

## Tasks Performed

### Task 1: Explore Amazon EC2 Dashboard

Explore the EC2 service dashboard in the AWS Management Console. Observe the different sections such as Instances, AMIs, Instance Types, Key Pairs, Security Groups, and Elastic IPs.

---

### Task 2: Launch an EC2 Instance

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type (t2.micro) under the free tier. Configure basic settings such as instance name, key pair, and security group.

---

### Task 3: Configure Security Group

Configure a security group to allow inbound access:

* SSH (Port 22) from your IP address
* HTTP (Port 80) from anywhere (0.0.0.0/0)

This security group acts as a firewall for the instance.

---

### Task 4: Connect to EC2 Instance

Connect to the running EC2 instance using SSH. Use the downloaded key pair and connect via terminal or PuTTY.

For Amazon Linux:

```
ssh -i "keyname.pem" ec2-user@<Public-IP>
```

---

### Task 5: Perform Basic Instance Operations

Perform the following operations from the EC2 console:

* Stop the instance
* Start the instance
* Reboot the instance

Observe the state changes of the instance.

---

### Task 6: Monitor EC2 Instance

Monitor the EC2 instance using the Monitoring tab. Observe metrics such as CPU utilization, network in/out, and instance status checks.

---

### Task 7: Terminate EC2 Instance

Terminate the EC2 instance after completing the experiment to avoid unnecessary AWS charges.

---

## Workflow (Student Explanation)

(Write the steps you followed in your own words)

1.The EC2 Dashboard was accessed through the AWS Management Console to explore the Amazon EBS volume types.

2.A new EBS volume was created by selecting the volume type, size, and the same Availability Zone as the EC2 instance.

3.The created EBS volume was attached to the running EC2 instance as an additional block device.

4.The attached volume was formatted using the ext4 file system and mounted to a directory in the EC2 instance.

5.Sample data was stored in the mounted volume, and after rebooting the instance, data persistence was verified successfully.



---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Dashboard / Instance List

<img width="1702" height="898" alt="image" src="https://github.com/user-attachments/assets/e8d3870b-bd4a-4946-ba31-2d38c288f418" />


---

### Screenshot 2: SSH Connection to Instance

<img width="936" height="343" alt="image" src="https://github.com/user-attachments/assets/503a1eb5-6ecb-499f-983a-6a43e200d75c" />


---

### Screenshot 3: Instance Monitoring / Status

<img width="1691" height="889" alt="image" src="https://github.com/user-attachments/assets/e975019a-d178-4fd6-a0c4-d0beb960313c" />

<img width="1678" height="889" alt="image" src="https://github.com/user-attachments/assets/11af4349-1d4f-4688-9246-a7bdfa12f61e" />



---

## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.
