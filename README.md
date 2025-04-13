# Level-2-CL-CY-Report

This is the report of the all the tasks completed in the level 2 of Computing and Cyber Security
---
🔗 **[CODES LINK](https://github.com/MithunSrinivas28/MARVEL-Codebase.git)**
---
# Task 1: AWS Lambda

#### What is AWS Lambda and Why is it Used?
AWS lambda is a severless compute sercive which helps to run the events or a code without a server.The users has to pay for the run time of the event or the application which helps in scalability and cost cutting. Its a paradigm shift in the field of cloud which helped to manage the servers in a better way



## Snippets of the task


Flowchar of the Deploying  a chat app in Aws lambda
![Lambda Task](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/lambda_task.jpg)
 
![List of API](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/List%20of%20api.jpeg)

![WebSocket Connected](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/socketconnected.png)



I learnt how to create a lambda fucntion ,websockets api and link them with different routes know as connect disconnect and sendMessage,I then connect the url with the help of Thunderclient API(i also tried it with Postman API)The below snippets shows that two users being connected

This task helped me to understand how to configure the aws lambdas and Api with permissions and environment variables. I also tried debugging 502 ERROR with the Cloud watch logs
### Output 
![Final Lambda Result](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/final_result_lambda.png)




---

# Task 2: Intoduction to Jenkins
Jenkins is a Tool which automates the process of building,,testing and deploying the software with a pipeline. It is fundamentally used for the Core concept fo Devops known as CI/CD .Jenkins is used to integrate the works and versions of a soft seamlessly and provide it to the end users.

![jenkins 1](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/jenkins%201)

![fd19fec6-f22a-49f3-8885-ab05d4580c20](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/fd19fec6-f22a-49f3-8885-ab05d4580c20.jpg)

## Key learnings
- I learnt the concept of CI/CD  and how it works in the the field of Devops
- I studied how to write a Jenkins file and implement it
- Got familar with using Jenkins
- I leant what are plugins and how they are used
  
### Task snippets 
![Jenkins Flow 3](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/jenkins%203.png)
![Jenkins Flow 4](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/jenkins%204.png)

I created a pipeline and wrote the stages for build,test and deploy.The jenkinsfile was used to automate these stages .I Ran the pipeline and executed these stages.


# Task 3:SSH

## What is SSH?
SSH is  a cryptographic network protocol for securing and managing access to the remote systems over and unsecured network. In other words, it is a network protocol that is used for transffering the data over the network.
![ssh flow](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/ssh%20flow.png)




---

### Task Performed
Below is a screenshot from the SSH key generation process:

![SSH Key Gen](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/ssh_key_gen.png)


Ultra mode
I used the `ssh-keygen` utility to generate a 4096-bit RSA key pair. This involved creating both a private and a public key, which are used for secure, password-less authentication to remote systems.

**Command used:**
bash
`ssh-keygen -t rsa -b 4096`

Successfully completed Bandit levels 0-5. Gained proficiency in basic SSH operations.Could not perform the SSH scripting task due to PowerShell command failures

### Learning SSH Commands

The following SSH commands were learned and used:
- `ssh username@hostname` – To connect to a remote server.
- `ssh -p <port> username@hostname` – To connect via a non-default port.
- `scp file user@host:path` – Securely copy files to a remote machine.
- `cat` – View file contents.
- `ls` – List files in a directory.
- `cd` – Change directory.
- `find` – Locate files.
- `du -sh *` – Check file sizes.

I utilized the `ssh-keygen -t rsa -b 4096` for the creation of a 4096-bit RSA key pair. The key pair that it created consisted of both a private and a public key. These keys are used for both 

`ssh-keygen -t rsa -b 4096`

Bandit levels 0-5 have been completed. Basic SSH operations were practiced. Could not perform the task with SSH scripting, since the Powershell command failed.

### Learning SSH Commands
"ssh username@hostname" This command is used to connect to a remote server.
SSH is for connecting without using the default port.
`scp` – Copy files to a different computer securely.
- `cat` – View file contents.
- `ls` – List files in a directory.
- `cd` – Change directory.
- `find` – Locate files.
- `du -sh *` – Check file sizes.

 # Bandit overtheiwre
 I completed bandit levels 0-5 and also learnt to complete level 13 and 18 which was related to the task(Writing a SSh script)

![Bandit Hidden File Solution](https://github.com/MithunSrinivas28/level-2-images/raw/main/level%202%20images/bandit.jpeg)

---

# Task 4: Terraform

## Terraform: What is it?
It is known as  Infrastructure as Code (IaC) and is used to define, provision, and manage cloud infrastructure. 
## **Execution of the task**  


I learned how to configure Terraform after installing it.I downloaded the required pluggings using the command `terraform init`.
I created a **Terraform configuration file** to specify the configuration of an AWS EC2 instance before deploying it. This involved choosing the instance type, Amazon Machine Image (AMI), and other important settings. After previewing the changes with `terraform plan`, I provisioned the instance using `terraform apply`. After it was successfully executed, I checked the instance's status in the **AWS Management Console** to make sure it
![Terraform Initialization](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/12499692-c065-4a8d-918b-13160503facb.jpg)  

![Terraform Applied Successfully](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/5c2fc8d5-1de4-429b-bac1-ce2d1012ce16.jpg)  

![Terraform Plan - EC2 Instance Creation](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/fc8ad240-40da-4d1a-8cd4-6e61caf80722.jpg)
### What I learnt 
- **Understanding Terraform Workflow:** Successfully navigated the process from initialization to deployment and teardown.  
- **EC2 Instance Deployment:** Created and managed an AWS EC2 instance using Terraform configurations.  
- **Terraform State Management:** Explored how Terraform tracks resources and maintains state consistency.  
- **Infrastructure Automation:** Learned how Terraform eliminates manual intervention, ensuring reliable infrastructure provisioning.  
- **Efficient Resource Management:** Practiced using `terraform destroy` to remove resources, optimizing cloud costs.  


# Task 5: Wireshark

### What is Wireshark?
Wireshark is a free and open-source packet analyzer used for capturing and inspecting network traffic in real-time. It helps diagnose network issues, analyze protocols, and detect security threats. Network administrators, cybersecurity professionals, and developers use it for troubleshooting, optimizing performance, and ensuring secure communications in various environments.

### What Did I Do in This Task?
I captured network traffic using Wireshark, applied filters to identify packet loss and retransmissions, and analyzed latency using round-trip time graphs. I examined TCP streams, used statistical tools to interpret data, and diagnosed network issues. Additionally, I saved results for further analysis to improve network performance and security monitoring.

![wireshark](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/wireshark.jpg)
 
![Wireshark Graph](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/wireshark%20graph.jpg)


# Task 6:Docker

### What is Docker?

Think of a **container** as a sealed box that holds your app and everything it depends on. This box works exactly the same wherever you open it—on your laptop, in a data center, or in the cloud
Docker is a tool that helps you package your application and everything it needs (code, libraries, and settings) into a **container**, so it can run the same way on any computer, server, or cloud.
## Docker Workflow
![docker workflow](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/docker%20workflow.png)
---
## Creating a Docker image
![creating a container](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/creating%20a%20container.png)
# Dockerfile Explanation
#### Defines a Base Image:
`FROM python:3.10-slim` → Uses a lightweight Python 3.10 image.
#### Sets the Working Directory:
`WORKDIR /app` → All commands will run inside `/app`.
#### Copies Files:
`COPY . .` → Copies all files from the current directory to the container.
#### Runs a Python Script:
`CMD ["python", "-c", "print('Hello from Docker!')"]` → Executes a one-liner Python script when the container starts.

---
# Task 7:Docker Spyware

## **1. What is Docker Spyware?**
Docker spyware is a **containerized application** designed to **monitor a folder for new files** (such as images) and automatically **send them to a remote server**. This concept is useful for:
- **Automated file monitoring**
- **Remote data transfer**
- **Surveillance and security applications**
---
## Watchdog in Python: Real-Time File System Monitoring
Python’s Watchdog module enables real-time monitoring of file system changes. It detects file creations, modifications, deletions, and movements using event handlers. Ideal for logging, automation, and security, Watchdog is widely used in file tracking, data pipelines, and intrusion detection for efficient and responsive system monitoring.

## **2. Task Summary**
### **What I Did:**
- Created a **Python script** to monitor a folder for new images.
- Built a **Docker container** to run the script.
- Tested the system by copying files to the monitored folder.
- Verified automatic file uploads and troubleshooting errors.

This setup is a Docker-based spyware simulation, where a script is actively watching a folder inside a container. Any new image added triggers an alert, indicating real-time surveillance on file changes
![spyware](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/spyware.png)

---
# Task 8:Web Scraping and Automation - Flight Ticket Price Analysis

In this task, I automated flight searching on Google Flights using Selenium. The process involved opening the website, entering departure and destination cities, selecting travel dates that is bengaluru to hyderabad, and triggering the search. I then extracted flight prices  and saved them in a CSV file for further analysis.

## Intro to dynamic webscraping
**Dynamic Scraping:** Extracting data from pages that load content dynamically using JavaScript (e.g., Selenium)
This is the reason we use selenium instead of beautifulsoup

![CSV BLR to HYD](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/csv_blr_to_hyd.jpg)

---


# Task 9:Hashing
###  What is Hashing?
Hashing is the process of converting input data (e.g., a password) into a fixed-length, unique hash value using a mathematical function. It is one-way, meaning the original input cannot be retrieved from the hash. Hashing is commonly used in password security, data integrity, and digital signatures.

### Why use hashing when its not reversible

The main purpose of hashing, especially when dealing with passwords or sensitive data, is to ensure security in case of unauthorized access, while still allowing for the verification of that data.

![hashing](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/hashing.png)
### What I Learned About Hashing
SHA-256 – A widely used cryptographic hash function that generates a 256-bit fixed-length hash.

Salting – Adding a random unique value (salt) to passwords before hashing to prevent attacks like rainbow tables.

PBKDF2 – A hashing method that applies multiple iterations (e.g., 100,000 rounds) to slow down brute-force attacks.

---
# Task 10:N Map
I got familiar with kali linux and Basic commands of Nmap.I learnt the importance of SSh and the types of penetration testing.I did scanning of of a target ip and found the open ports and their version

Ping
`ping` command is a network utility used to test the **reachability** of a host on an IP network. It is commonly used to check if a particular system (device, server, or host) is online and responding to network requests.

![Pasted image 20241023162006](https://github.com/user-attachments/assets/a0bbddcb-3c45-4e1f-9fb5-ad33c79dc073)

  ### SN command

The `-sn` option is used to perform a **ping scan** (also known as a "no port scan"). When you use this option, Nmap disables the default port scanning phase and instead focuses on **host discovery**. It checks whether the hosts on the network are up (alive) without probing their open ports.
![Pasted image 20241023180758](https://github.com/user-attachments/assets/81e38c11-ff09-464e-b7fc-c8122d0c62c6)

