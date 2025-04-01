# Level-2-CL-CY-Report
This is the report of the all the tasks completed in the level 2 of Computing and Cyber Security


# Task 1: AWS Lambda

#### What is AWS Lambda and Why is it Used?
AWS Lambda is a serverless compute service that automatically runs code in response to events, managing infrastructure and scaling automatically. It is used for event-driven applications, automation, and microservices without provisioning or managing servers.

I deployed a basic AWS Lambda function that returns "Hello, World!" using Python. I configured the function.I learned how to create, deploy, and test AWS Lambda functions, configure IAM roles for execution permissions, and understand event-driven execution models. I also gained familiarity with the AWS Lambda management console and function triggers.
![628d06df-9131-4adb-8047-6c6d67ed43c5](https://github.com/user-attachments/assets/0ff96918-5589-488e-9723-90cbbe48f181)

![f4a4c57f-f9d1-4cf1-a7b2-e343269516d9](https://github.com/user-attachments/assets/858fcccf-8b88-4476-a10a-1b636e7978ea)

  

# Task 2: Intro to Jenkins!

Jenkins is like a **highly efficient personal assistant** in a busy kitchen. It automates the process of building, testing, and deploying your software (the dishes), following a recipe (pipeline) to make sure everything gets done properly. It uses specialized tools (plugins) to speed things up and gives you feedback on how well everything went, ensuring that your software gets to your customers (end-users) seamlessly.
![Jenkins flowchart](https://github.com/user-attachments/assets/728dc650-0be0-498a-9c2d-399f5be20bfd)


## Flowchart Explanation:
Developer → Writes and updates code in a local environment.

Code Repository → The developer pushes the code to a version control system (e.g., GitHub, GitLab).

Jenkins → Detects the code change and triggers a pipeline (automated process).

Artifact Repository → If the build is successful, Jenkins stores artifacts (e.g., JAR, WAR files) in a repository like Nexus or JFrog Artifactory.

Deployment → The built application is deployed to a staging/production server (e.g., AWS, Kubernetes).

Test Reports → Jenkins runs automated tests and generates reports to verify if the application is working correctly.

I installed Jenkins, created a pipeline, and defined stages for Build, Test, and Deploy. I wrote a Jenkinsfile to automate these steps. Then, I ran the pipeline in Jenkins, which executed each stage sequentially. Finally, Jenkins successfully completed the pipeline, confirming the CI/CD process was set up correctly. 🚀
[Jenkins pipeline code](https://github.com/MithunSrinivas28/MARVEL-Codebase.git)

# Task 5: Wireshark

### What is Wireshark?
Wireshark is a free and open-source packet analyzer used for capturing and inspecting network traffic in real-time. It helps diagnose network issues, analyze protocols, and detect security threats. Network administrators, cybersecurity professionals, and developers use it for troubleshooting, optimizing performance, and ensuring secure communications in various environments.

### Why is Wireshark Used?
Wireshark is used for network troubleshooting, security analysis, and performance optimization. It helps identify latency, packet loss, and retransmissions. Administrators use it to analyze protocols, detect cyber threats, and debug communication issues. Its graphical interface and filtering options make diagnosing problems easier, ensuring efficient network monitoring and performance tuning.

### What Did I Do in This Task?
I captured network traffic using Wireshark, applied filters to identify packet loss and retransmissions, and analyzed latency using round-trip time graphs. I examined TCP streams, used statistical tools to interpret data, and diagnosed network issues. Additionally, I saved results for further analysis to improve network performance and security monitoring.

![a828abc4-31fc-4c39-b3a3-10db49d1dcae](https://github.com/user-attachments/assets/4d7962a3-db02-40fb-8a27-1579cc4daa08)




# Task 6:Docker


### What is Docker?

Think of a **container** as a sealed box that holds your app and everything it depends on. This box works exactly the same wherever you open it—on your laptop, in a data center, or in the cloud

Docker is a tool that helps you package your application and everything it needs (code, libraries, and settings) into a **container**, so it can run the same way on any computer, server, or cloud.

I learned to create a Docker container and image by following these steps:

1.Write a Dockerfile – Defined the base image, dependencies, and commands.

2.Build the image – Used docker build -t my_image . to create a reusable image.

3.Run a container – Used docker run -d --name my_container my_image to start a container from the image.

4.Check running containers – Used docker ps to list active containers.

5.Push the image – Uploaded it to Docker Hub using docker push my_repo/my_image.


# Task 7:Docker Spyware


## **1. What is Docker Spyware?**
Docker spyware is a **containerized application** designed to **monitor a folder for new files** (such as images) and automatically **send them to a remote server**. This concept is useful for:
- **Automated file monitoring**
- **Remote data transfer**
- **Surveillance and security applications**
---

## **2. Task Summary**
### **What We Did:**
- Created a **Python script** to monitor a folder for new images.
- Built a **Docker container** to run the script.
- Tested the system by copying files to the monitored folder.
- Verified automatic file uploads and troubleshooting errors.

## **4. Task Process**
1. **Created a Python script** (`monitor.py`) to detect and upload images.
2. **Wrote a Dockerfile** to containerize the script.
3. **Built and ran the container** using:
   ```sh
   docker build -t spyware_simulation .
   docker run -d --name spyware_container spyware_simulation
   ```
4. **Tested file monitoring** by copying an image into the container:
   ```sh
   docker cp bird.jpg spyware_container:/app/monitored_folder
   ```
5. **Checked logs** to confirm automatic upload:
   ```sh
   docker logs spyware_container
   ```
6. **Debugged issues** using:
   ```sh
   docker restart spyware_container
   docker exec -it spyware_container python /app/monitor.py
   ```

# Task 8:Web Scraping and Automation - Flight Ticket Price Analysis

In this task, I automated flight searching on Google Flights using Selenium. The process involved opening the website, entering departure and destination cities, selecting travel dates, and triggering the search. We then extracted flight prices and saved them in a CSV file for further analysis.

Key libraries used were Selenium (for browser automation), pandas (for handling CSV files), and time (for adding necessary delays). A crucial aspect was handling dynamic elements with WebDriverWait to ensure smooth execution. Additionally, using XPath for locating elements proved essential for interacting with the page.

#### I couldn't scrape the flight ticket prices due to Google's anti-bot protection, so I used Selenium to capture an image of the website after the automation was completed.

![google_flights_results](https://github.com/user-attachments/assets/548df9e2-849b-417b-be43-2f1159af6aa2)



# Task 9:Hashing
###  What is Hashing?
Hashing is the process of converting input data (e.g., a password) into a fixed-length, unique hash value using a mathematical function. It is one-way, meaning the original input cannot be retrieved from the hash. Hashing is commonly used in password security, data integrity, and digital signatures.

#### The image shows a Python program for user authentication using hashed passwords. Users register and log in, with passwords stored securely in passwords.txt. The terminal confirms successful registration and login for users Marvel and UVCE.
![image](https://github.com/user-attachments/assets/98ee0515-12aa-43b3-be81-9fb6020e08f2)

### What I Learned About Hashing
SHA-256 – A widely used cryptographic hash function that generates a 256-bit fixed-length hash.

Salting – Adding a random unique value (salt) to passwords before hashing to prevent attacks like rainbow tables.

PBKDF2 – A hashing method that applies multiple iterations (e.g., 100,000 rounds) to slow down brute-force attacks.

### Password Hashing Process

- Generate a random salt.
- Hash the password with SHA-256 & PBKDF2.
- Store the salt + hash for verification.
- During login, recompute the hash with the stored salt and compare it to the stored hash.


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

Ping Scan (-sP): Discovers live hosts on a network by checking which IP addresses are active without scanning ports.

Stealth Scan (-sS): Performs a SYN scan, which is faster and less likely to be detected by firewalls compared to a full connection scan.

OS Detection (-O): Tries to determine the target’s operating system by analyzing network responses.

Specific Port Scan (-p): Targets specific port(s) on the host instead of scanning all commonly used ports.

Aggressive Scan (-A): Combines multiple scan types, including OS detection, version detection, script scanning, and traceroute.
