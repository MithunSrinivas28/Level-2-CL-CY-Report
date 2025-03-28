# Level-2-CL-CY-Report
This is the report of the all the tasks completed in the level 2 of Computing and Cyber Security

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


## What is Docker?

Think of a **container** as a sealed box that holds your app and everything it depends on. This box works exactly the same wherever you open it—on your laptop, in a data center, or in the cloud

Docker is a tool that helps you package your application and everything it needs (code, libraries, and settings) into a **container**, so it can run the same way on any computer, server, or cloud.
