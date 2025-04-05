# Level-2-CL-CY-Report

This is the report of the all the tasks completed in the level 2 of Computing and Cyber Security
---
###  The Code Lives Here 💾.

🔗 **[MARVEL-Codebase](https://github.com/MithunSrinivas28/MARVEL-Codebase.git)**
---
# Task 1: AWS Lambda

#### What is AWS Lambda and Why is it Used?
AWS Lambda is a serverless compute service that automatically runs code in response to events, managing infrastructure and scaling automatically. It is used for event-driven applications, automation, and microservices without provisioning or managing servers.

I deployed a basic AWS Lambda function that returns "Hello, World!" . I configured the function.I learned how to create, deploy, and test AWS Lambda functions . I also gained familiarity with the AWS Lambda management console and function triggers.

![aws sucess](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/aws%20sucess.jpg)
![function code](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/function%20code.jpg)

---

# Task 2: Intro to Jenkins!

Jenkins is like a **highly efficient personal assistant** in a busy kitchen. It automates the process of building, testing, and deploying your software (the dishes), following a recipe (pipeline) to make sure everything gets done properly. It uses specialized tools (plugins) to speed things up and gives you feedback on how well everything went, ensuring that your software gets to your customers (end-users) seamlessly.

![jenkins 1](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/jenkins%201)

![fd19fec6-f22a-49f3-8885-ab05d4580c20](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/fd19fec6-f22a-49f3-8885-ab05d4580c20.jpg)

## Flowchart Explanation:

1. **Developers** commit code to a **repository**.
2. The **CI Server** fetches the code and runs tests.
3. If tests **fail**, developers get feedback to fix errors.
4. If tests **pass**, the build moves to **Testers**.
5. Testers validate and report issues if found.
6. If successful, the build proceeds to **Release & Deploy**.
7. Ensures **automation, faster feedback, and smoother deployments**.

### Task snippets 
![Jenkins Flow 3](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/jenkins%203.png)
![Jenkins Flow 4](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/jenkins%204.png)

I installed Jenkins, created a pipeline, and defined stages for Build, Test, and Deploy. I wrote a Jenkinsfile to automate these steps. Then, I ran the pipeline in Jenkins, which executed each stage sequentially. Finally, Jenkins successfully completed the pipeline, confirming the CI/CD process was set up correctly. 🚀

# Task 3:SSH

## What is SSH?
SSH (**Secure Shell**) is a cryptographic network protocol for securely accessing and managing remote systems over an unsecured network. It provides encrypted communication, authentication, and file transfer. SSH replaces insecure protocols like Telnet and supports key-based authentication, tunneling, and remote command execution, making it essential for secure server administration.

![ssh flow](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/ssh%20flow.png)


I focused on the generation and handling of SSH key pairs using standard command-line tools. This exercise helped me understand the practical foundations of authentication and secure communication over SSH.

---

### Task Performed
Below is a screenshot from the SSH key generation process:

![SSH Key Generation Screenshot](https://github.com/MithunSrinivas28/level-2-images/raw/main/level%202%20images/image.png)

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

### OverTheWire Bandit 
Successfully completed Bandit levels 0-5,13,18. Gained proficiency in basic SSH operations.Could not perform the SSH scripting task due to PowerShell command failures
#### Bandit Level - Hidden File
The following screenshot shows the solution where the user accesses a hidden file `.hidden` inside the `inhere` directory.

![Bandit Hidden File Solution](https://github.com/MithunSrinivas28/level-2-images/raw/main/level%202%20images/bandit.jpeg)

---

# Task 4: Terraform

## What is Terraform
Terraform is an open-source **Infrastructure as Code (IaC)** tool that allows users to define and provision cloud resources in a **declarative** manner. Unlike traditional provisioning methods, Terraform automates the entire process, ensuring consistency, scalability, and efficiency. It supports multiple cloud providers such as AWS, Azure, and Google Cloud, making it a preferred choice for cloud infrastructure management.

**Helpful analogy for it:**
Terraform is like a cab driver for your cloud infrastructure.

You tell it where to go (define resources), it plans the best route (terraform plan), and drives you there (terraform apply). If you change your destination (update infra), it adjusts. When the trip is over, you end it (terraform destroy).

## **Task Execution**  
I installed Terraform and configured it to interact with AWS. The process began with **Terraform initialization**, where I used the command `terraform init` to download and set up necessary provider plugins. Following this, I configured AWS credentials to allow Terraform to create resources in my AWS account.

To deploy an AWS EC2 instance, I defined its configuration in a **Terraform configuration file**. This included specifying the Amazon Machine Image (AMI), instance type, and other key parameters. I then used `terraform plan` to preview the changes and `terraform apply` to provision the instance. Upon successful execution, I verified the instance's status in the **AWS Management Console**, confirming that it was running.

To clean up, I executed `terraform destroy`, which safely removed all deployed infrastructure. This step is crucial in cloud environments to prevent unnecessary resource consumption and costs.
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
#### Docker container 
  `docker run --rm my-python-app`
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

In this task, I automated flight searching on Google Flights using Selenium. The process involved opening the website, entering departure and destination cities, selecting travel dates, and triggering the search. We then extracted flight prices and saved them in a CSV file for further analysis.

Key libraries used were Selenium (for browser automation), pandas (for handling CSV files), and time (for adding necessary delays). A crucial aspect was handling dynamic elements with WebDriverWait to ensure smooth execution. Additionally, using XPath for locating elements proved essential for interacting with the page.

## Intro to dynamic webscraping
**Dynamic Scraping:** Extracting data from pages that load content dynamically using JavaScript (e.g., Selenium)
This is the reason we use selenium instead of beautifulsoup

#### Google Flights has strong anti-bot protection mechanisms, including dynamic content loading, CAPTCHA, and request blocking. These protections prevent automated scripts from accessing structured data directly. Instead of scraping, I used Selenium to take a screenshot as an alternative method to capture information.

![screenshot](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/screenshot.png)
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

### Password Hashing Process

- Generate a random salt.
- Hash the password with SHA-256 & PBKDF2.
- Store the salt + hash for verification.
- During login, recompute the hash with the stored salt and compare it to the stored hash.

---
# Task 10:N Map
I got familiar with kali linux and Basic commands of Nmap.I learnt the importance of SSh and the types of penetration testing.I did scanning of of a target ip and found the open ports and their versions
## KALI Linux commands

### Sudo command 
  In **Kali Linux** (and other Linux distributions), the `sudo` (short for "superuser do") command allows a permitted user to execute a command as the **superuser** (root) or another user, as specified by the security policy. It is primarily used for administrative tasks that require higher privileges than a normal user account.
![Pasted image 20241023150909](https://github.com/user-attachments/assets/4813f710-c3ec-42a9-8040-cbc584c4774a)

Ping
`ping` command is a network utility used to test the **reachability** of a host on an IP network. It is commonly used to check if a particular system (device, server, or host) is online and responding to network requests.

![Pasted image 20241023162006](https://github.com/user-attachments/assets/a0bbddcb-3c45-4e1f-9fb5-ad33c79dc073)

  ### SN command

The `-sn` option is used to perform a **ping scan** (also known as a "no port scan"). When you use this option, Nmap disables the default port scanning phase and instead focuses on **host discovery**. It checks whether the hosts on the network are up (alive) without probing their open ports.
![Pasted image 20241023180758](https://github.com/user-attachments/assets/81e38c11-ff09-464e-b7fc-c8122d0c62c6)

