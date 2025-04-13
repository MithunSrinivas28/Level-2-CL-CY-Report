# Level-2-CL-CY-Report

This is the report of the all the tasks completed in the level 2 of Computing and Cyber Security
---
🔗 **[CODES LINK](https://github.com/MithunSrinivas28/MARVEL-Codebase.git)**
---
# Task 1: AWS Lambda

#### What is AWS Lambda and Why is it Used?
AWS lambda is a severless compute service which helps to run the events or a code without a server.The user has to pay for the run time of the event or the application ,this feature helps in scalability and cost cutting. Its a paradigm shift in the field of cloud which helped to manage the servers in a better way.



## Snippets of the task


Flowchart of the Deploying  a chat app in Aws lambda
![Lambda Task](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/lambda_task.jpg)
 
![List of API](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/List%20of%20api.jpeg)

![WebSocket Connected](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/socketconnected.png)

## Key learnings

I learnt how to create a lambda fucntion ,websockets api and link them with different routes know as connect disconnect and sendMessage,I then connected the url with the help of Thunderclient API(i also tried it with Postman API)The below snippets shows that two users being connected

This task helped me to understand how to configure the aws lambdas and Api with permissions and environment variables. I also tried debugging 502 ERROR with the Cloud watch logs
### Output 
![Final Lambda Result](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/final_result_lambda.png)




---

# Task 2: Intoduction to Jenkins
Jenkins is a Tool which automates the process of building,,testing and deploying the software with a pipeline. It helps to understand the fundamental concept fo Devops known as CI/CD .Jenkins is used to integrate the works and versions of a software seamlessly and provide it to the end users.

![jenkins 1](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/jenkins%201)

![fd19fec6-f22a-49f3-8885-ab05d4580c20](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/fd19fec6-f22a-49f3-8885-ab05d4580c20.jpg)

## Key learnings
- I learnt the concept of CI/CD  and how it works in the the field of Devops.
- I studied how to write a Jenkins file and implement it.
- Got familar with using Jenkins.
- I leant what are plugins and how they are used.
  
### Task snippets 
![Jenkins Flow 3](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/jenkins%203.png)
![Jenkins Flow 4](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/jenkins%204.png)

I created a pipeline and wrote the stages for build,test and deploy.The jenkinsfile was used to automate these stages .I ran the pipeline and executed these stages.


# Task 3:SSH

## What is SSH?
SSH is  a cryptographic network protocol for securing and managing access to the remote systems over and unsecured network. In other words, it is a network protocol that is used for transffering the data over the network.
![ssh flow](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/ssh%20flow.png)




---

### Task Performed
Below is a screenshot from the SSH key generation process:

![SSH Key Gen](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/ssh_key_gen.png)

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
It is known as  Infrastructure as Code (IaC) and is used to define, provision, and manage cloud infrastructure. It allows users to write declarative configuration files specifying the desired state of infrastructure, and Terraform handles the deployment and changes.
## **Execution of the task**  


I learned how to configure Terraform after installing it.I downloaded the required pluggings using the command `terraform init`.
. After previewing the changes with `terraform plan`, I provisioned the instance using `terraform apply`. After it was successfully executed, I checked the instance's status in the **AWS Management Console** to make sure it worked
![Terraform Initialization](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/12499692-c065-4a8d-918b-13160503facb.jpg)  

![Terraform Applied Successfully](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/5c2fc8d5-1de4-429b-bac1-ce2d1012ce16.jpg)  

![Terraform Plan - EC2 Instance Creation](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/fc8ad240-40da-4d1a-8cd4-6e61caf80722.jpg)
###  Key learnings 
- I unserstood The terraform workflow
- I learnt how to create and ec2 instance(I created a ubuntu instance from AIM)
- I understood some of the importnat terraform commands and implemented it

# Task 5: Wireshark

### What is Wireshark?
Wireshark is a free open source toll which is used to analyse the data packets in a particular newtork. It is mainly useful for threat detection and controlling traffic in a particular network

### What Did I Do in This Task?
I captured my own Wifi netwrok  and analysed and understood the different ascpets of the captured data with various inbuilt tools in Wireshark Itself
I Filtered out certain protocols like tcp and http and analysed them by plotting graphs and seeing the consevations between ports witht the help of different tools


![wireshark](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/wireshark.jpg)
 
![Wireshark Graph](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/wireshark%20graph.jpg)


# Task 6:Docker

### What is Docker?

Docker is a tool in which you cna pack your application into a container including all its versions.You can run your docker container in any system without installing your application into the OS again 
## Docker Workflow
![docker workflow](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/docker%20workflow.png)
---
## Creating a Docker image
![creating a container](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/creating%20a%20container.png)

## Key learnings
- I learnt the concept of how docker works
- I basically understood how to write a dockerfile
- I learnt how to create a docker container with the help of dockerfile
---
# Task 7:Docker Spyware

## 1. What is Docker Spyware?
Docker spyware is the extened task of docker cretaion where a pyton spyware is being setup with the help of the python library known as Watchdog. the python code is linked the the docker container which monitors the changes that is being done in the dcoker container.I very useful tool that detect threats and changes done in the particuar container

 
--

## Key learnings
- I learnt how to work with the watchdog library
- I learnt how to build a docker container
- Tested the system by adding an image into the file
- Created a spyware that could monitor my container

This is the code snippet of the spyware which detects that the BIRD image is being added to the container
![spyware](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/spyware.png)

---
# Task 8:Web Scraping and Automation - Flight Ticket Price Analysis

In this task, I automated flight searching on Google Flights using Selenium. The process involved opening the website, entering departure and destination cities, selecting travel dates that is bengaluru to hyderabad, and triggering the search. I then extracted flight prices  and saved them in a CSV file for further analysis.

## Intro to dynamic webscraping

The dynamic webscraping includes penetrating thorugh Javascript parts of the websites The selenium libarary used in the task is a dynamic tool whereas the Beautifulsoup used in the previous level is a static webscraper which only reads the HTML.

![CSV BLR to HYD](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/csv_blr_to_hyd.jpg)

---


# Task 9:Hashing
###  What is Hashing?
Hashing is a one way tool which is used to secure passwords and verify them without withdrawing the original data .Hashing refers to the process of generating a fixed-size output from an input of variable size using the mathematical formulas known as hash functions.

![hashing](https://raw.githubusercontent.com/MithunSrinivas28/level-2-images/main/level%202%20images/hashing.png)
### What I Learned About Hashing

-I learnt how SHA 256 algorithm works and the math behind it.
- I learnt why salting is used and how it make the hashing process my secure
- I implemented a basic hashing script which stores the password of the users
- I understood that no hashed data is same even though the text might be similar

---
# Task 10:N Map
I got familiar with kali linux and Basic commands of Nmap.I learnt the importance of SSh and the types of penetration testing.I did scanning of of a target ip and found the open ports and their version

Ping
` It is commonly used to check if a particular system (device, server, or host) is online and responding to network requests.

![Pasted image 20241023162006](https://github.com/user-attachments/assets/a0bbddcb-3c45-4e1f-9fb5-ad33c79dc073)

  ### SN command

The `-sn` option is used to perform a **ping scan** (also known as a "no port scan").It checks whether the hosts on the network are up (alive) without probing their open ports.
![Pasted image 20241023180758](https://github.com/user-attachments/assets/81e38c11-ff09-464e-b7fc-c8122d0c62c6)

