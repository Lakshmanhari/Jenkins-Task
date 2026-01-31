JENKINS SETUP AND BASIC OPERATIONS USING AWS EC2
===============================================

TASK DESCRIPTION:
-----------------
Launch Jenkins on an AWS EC2 instance and explore basic Jenkins operations such as
creating projects (jobs) and managing users.

TECH STACK USED:
----------------
- AWS EC2
- Jenkins
- Ubuntu 22.04 LTS
- Java (OpenJDK 21)

-------------------------------------------------

OBJECTIVE:
----------
The objective of this task is to understand how Jenkins is installed and configured
on a cloud server and how it is used to create automation projects and manage users.

-------------------------------------------------

STEPS PERFORMED:
----------------

1. EC2 INSTANCE CREATION:
   - Created an EC2 instance using Ubuntu 22.04 LTS
   - Instance Type: t3.micro
   - Opened ports:
     - 22 (SSH)
     - 8080 (Jenkins Web UI)

2. CONNECTED TO EC2:
   - Used EC2 connect for connection

3. JENKINS INSTALLATION:
   - Updated system packages
   - Installed OpenJDK 17
   - Added Jenkins repository and key
   - Installed Jenkins
   - Started and enabled Jenkins service

4. JENKINS ACCESS:
   - Accessed Jenkins via browser using:
     http://<EC2-Public-IP>:8080
   - Retrieved initial admin password
   - Installed suggested plugins
   - Created admin user

5. PROJECT (JOB) CREATION:
   - Created a Freestyle Project
   - Added shell build step:
     echo "Hello from Jenkins"
   - Triggered build manually
   - Verified output in console logs

6. USER MANAGEMENT:
   - Enabled Jenkins internal user database
   - Created a new user
   - Assigned role-based permissions
   - Verified access by logging in as new user

-------------------------------------------------

RESULT:
-------
- Jenkins was successfully launched on AWS EC2
- A Jenkins project was created and executed successfully
- Multiple users were created and managed with permissions

-------------------------------------------------

