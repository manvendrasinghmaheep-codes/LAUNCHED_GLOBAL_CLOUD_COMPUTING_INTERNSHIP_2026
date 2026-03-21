# LAB SESSIONS: BEGINNING OF CLOUD COMPUTING INTERNSHIP

The lab sessions marked the foundation of my cloud computing internship, where I transitioned from theoretical understanding to hands-on implementation. These initial experiments were not just about learning tools, but about understanding how modern cloud infrastructure operates in real-world scenarios. From setting up my first cloud environment to launching EC2 instances, each step contributed to building a practical mindset required in the field of cloud engineering. This phase played a crucial role in shaping my approach toward problem-solving, debugging, and working with AWS.

Through these sessions, I explored the core concepts of cloud computing by actively working on services and understanding how virtual servers can be configured, accessed, and managed remotely. The experience of working with different operating systems including Windows, Linux, and Ubuntu provided a deeper insight into system-level operations within the cloud. These labs not only strengthened my technical base but also prepared me to handle more complex, real-world cloud projects in the later stages of the internship.

# INTRODUCTION TO CLOUD COMPUTING

Computing is the process of utilizing computer technology to complete a task.
For example - Storing, Coding, Gaming, etc.

## EVOLUTION OF CLOUD COMPUTING

### 1. DESKTOP COMPUTING
A model where apps and processes run directly on PCs or workstation where each computer operates and manages resources locally. Better for small tasks but limited to hardware and doesn't support resource sharing with other systems.
### 2. CLIENT-SERVER COMPUTING
Network architecture where a central server hosts and provides resources and services, such as data, apps and files to multiple client devices. Client initiate requests to access resources to which server processes and then responds to the requests. 
### 3. CLUSTER COMPUTING 
It involves linking multiple computers known as nodes to work as  a single powerful system. Those nodes are typically in the same location and connected through a high speed network. Cluster computing provides redundancy and improved processing speed, often used in data centres, scientifiic research and financial modelling. Unlike grid computing, cluster nodes are highly coupled and work together on tasks with inter-dependent processing needs.
### 4. GRID COMPUTING
Grid computing is a distributed computing model where resources such as power, storage and processing are pooled from multiple computers often across different locations to solve complex tasks. Each computer or node work on small part of the task and results are aggregated at the end. Grid computing is ideal for large scale scientific or engineering problems, as it enables high performance computing by levaraging resouces accross a network.
### 5. CLOUD COMPUTING
It is a model where computing resources such as storage, applications and processing power are provided over the internet by third party providers. Resources are dynamically allocated allowing users to scale up or scale down based on demand. Cloud computing provides flexibility as users can access services without managing underlying infrastructure making it suitable for wide range of apps from personal to enterprise level workloads.
### FAMOUS AMAZON PROBLEM

In the early 2000s, Amazon faced significant challenges in managing its rapidly growing infrastructure as its global retail operations expanded. The company had to invest heavily in servers, storage systems, and data centers to handle peak traffic, especially during seasonal events. This resulted in high capital expenditure and inefficient resource utilization, as many servers remained underused during non-peak periods. Managing such large-scale infrastructure also increased operational complexity and maintenance costs.

During this time, concepts promoted by organizations like the National Institute of Standards and Technology (NIST) emphasized the idea of on-demand resource availability and scalable computing. Inspired by these ideas, Amazon identified an opportunity to convert its internal infrastructure into a service that could be rented by other businesses. This led to the creation of Amazon Web Services (AWS), marking the beginning of cloud computing as a commercial, scalable, and pay-as-you-go model.

## BENEFITS OF CLOUD COMPUTING

### 1. COST EFFICIENCY
#### REDUCED INFRASTRUCTURE COSTS
Cloud computing eliminates the need for organizations to invest in expensive physical hardware such as servers, storage devices, and networking components. Instead of large upfront capital expenditures, businesses can rely on cloud providers to supply infrastructure on demand. This significantly reduces the financial burden, especially for startups and small-scale enterprises, allowing them to allocate resources more efficiently toward growth and innovation.

#### REDUCTION OF OPERATIONAL COSTS
In addition to infrastructure savings, cloud computing reduces operational costs by minimizing the need for in-house IT teams and maintenance efforts. Tasks such as hardware upgrades, system monitoring, and troubleshooting are managed by cloud providers. This allows organizations to focus on core business operations while benefiting from professionally managed, highly efficient cloud environments.

---

### 2. SCALABILITY
#### ELASTIC RESOURCES
Cloud platforms provide the ability to scale resources up or down based on demand. This elasticity ensures that applications can handle varying workloads without performance degradation. Businesses can increase computing power during peak demand and reduce it during low usage periods, ensuring optimal resource utilization and cost savings.

#### GLOBAL REACH
Cloud services are distributed across multiple geographic regions, enabling organizations to deploy applications globally with ease. This allows businesses to serve users from different parts of the world with reduced latency and improved performance, enhancing user experience and expanding market reach.

---

### 3. FLEXIBILITY AND AGILITY
#### QUICK PROVISIONING
Cloud computing enables rapid deployment of resources, allowing developers and organizations to launch applications within minutes. This significantly reduces development time and accelerates innovation cycles, making it easier to respond to changing market demands.

#### SUPPORT FOR DIVERSE WORKLOAD
Cloud platforms support a wide range of workloads, including web applications, data analytics, machine learning, and enterprise software. This flexibility allows businesses to experiment with new technologies and adapt quickly to evolving requirements.

---

### 4. SECURITY
#### ADVANCED SECURITY FEATURES
Cloud providers implement robust security mechanisms such as encryption, identity management, and multi-factor authentication. These features help protect sensitive data from unauthorized access and cyber threats, ensuring a secure computing environment.

#### COMPLIANCES OF HIPAA ETC.
Leading cloud providers comply with global regulatory standards such as HIPAA, GDPR, and ISO certifications. This ensures that organizations can meet legal and compliance requirements while handling sensitive data in industries like healthcare and finance.

---

### 5. DISASTER RECOVERY AND BUSINESS CONTINUITY
#### DATA BACKUP AND RECOVERY
Cloud computing offers automated backup solutions that ensure data is securely stored and easily recoverable in case of system failures or data loss. This minimizes downtime and protects critical business information.

#### HIGH AVAILABILITY
Cloud platforms are designed with redundancy and failover mechanisms, ensuring high availability of applications and services. Even if one server fails, workloads are automatically shifted to another, maintaining uninterrupted operations.

---

### 6. COLLABORATION AND REMOTE WORK
#### ACCESS FROM ANYWHERE
Cloud services enable users to access applications and data from any location with an internet connection. This supports remote work environments and enhances productivity by allowing seamless access to resources.

#### REAL-TIME COLLABORATION
Teams can collaborate in real-time using cloud-based tools, enabling multiple users to work on the same project simultaneously. This improves efficiency, communication, and overall project management.

---

### 7. AUTOMATIC SOFTWARE UPDATES
#### MODERNITY
Cloud providers handle software updates, security patches, and system upgrades automatically. This ensures that users always have access to the latest features and technologies without manual intervention, keeping systems modern and secure.

---

### 8. INNOVATION
#### ACCESS TO ADVANCED TOOLS
Cloud platforms provide access to advanced technologies such as artificial intelligence, machine learning, and big data analytics. This empowers organizations to innovate and build intelligent applications without requiring specialized infrastructure.

#### PROTOTYPING AND TESTING
Developers can quickly create and test prototypes in cloud environments without significant investment. This encourages experimentation and reduces the risk associated with developing new solutions.

---

### 9. ENVIRONMENTAL SUSTAINABILITY
#### EFFICIENT RESOURCE UTILISATION
Cloud computing promotes efficient use of resources by sharing infrastructure among multiple users. This reduces energy consumption and carbon footprint compared to traditional data centers, contributing to environmental sustainability.

---

### 10. PERFORMANCE OPTIMIZATION
#### HIGH PERFORMANCE COMPUTING
Cloud platforms offer high-performance computing capabilities that enable faster data processing and improved application performance. This is especially useful for complex computations and large-scale workloads.

#### LOAD BALANCING
Cloud systems use load balancing techniques to distribute traffic evenly across servers. This ensures optimal performance, prevents system overload, and enhances reliability of applications.

## CLOUD DEPLOYMENT MODELS

### PUBLIC CLOUD
Public cloud refers to cloud services that are delivered over the internet and shared among multiple users. These services are managed by third-party providers and offer high scalability and cost efficiency. Users can access resources on a pay-as-you-go basis without worrying about infrastructure management.

### PRIVATE CLOUD
Private cloud is dedicated to a single organization and provides enhanced security and control over resources. It can be hosted on-premises or by a third-party provider. This model is suitable for organizations with strict data privacy and compliance requirements.

### HYBRID CLOUD
Hybrid cloud combines both public and private cloud environments, allowing data and applications to be shared between them. This provides flexibility, enabling organizations to use public cloud for scalability while maintaining sensitive data in a private cloud.

## CLOUD SERVICE MODELS

### ON SITE
On-site or traditional computing involves managing all hardware, software, networking, and storage within an organization’s physical infrastructure. The organization is responsible for installation, maintenance, and security. While it provides full control, it requires high investment and ongoing operational effort.

### IAAS
Infrastructure as a Service (IaaS) provides virtualized computing resources such as servers, storage, and networking over the internet. Users have control over operating systems and applications, while the cloud provider manages the underlying hardware. It offers flexibility and scalability for various workloads.

### PAAS
Platform as a Service (PaaS) provides a complete development environment including operating systems, databases, and development tools. Developers can focus on building applications without worrying about infrastructure management, making development faster and more efficient.

### SAAS
Software as a Service (SaaS) delivers software applications over the internet on a subscription basis. Users can access applications through web browsers without installation or maintenance. The provider manages everything, including updates, security, and infrastructure.

## INSTANCES AND INSTANCE TYPES

An instance in cloud computing refers to a virtual server that runs applications in a cloud environment. These instances are created using virtualization technology, allowing multiple virtual machines to operate on a single physical server. Instances can be configured with different combinations of CPU, memory, storage, and networking capabilities based on the requirements of the application. They provide flexibility, scalability, and cost efficiency by allowing users to pay only for the resources they use.

Cloud providers offer various instance families designed for specific use cases. General purpose instances (M, T) provide balanced resources, compute optimized instances (C) are designed for high-performance processing, memory optimized instances (R, X) handle large datasets, storage optimized instances (D, H) support high disk throughput, and accelerated computing instances (P, G, F) are used for machine learning and graphics-intensive tasks.

## AWS ENVIRONMENT SETUP
After gaining initial exposure to fundamental, technical and historical aspects of cloud computing it was the time for me to move towards my first hands on practical on Amazon Web Services (AWS), which began with the creation of my aws account and exploring it's dashboard section with the help of AWS Management Console which serves as central interface for all cloud services.


<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/AWS%20Account%20Creation.png" width="800"/>
</p>

<p align="center"><em>Figure 1: AWS Management Console dashboard displaying core services and navigation panel.</em></p>


### AWS ACCOUNT CREATION 
#### HERE ARE THE STEPS BY WHICH MY ACCOUNT WAS CREATED AND PROTECTED:
IT IS RECOMMENDED TOO USE LAPTOP FOR PROPER AWS CONSOLE, HOSTING AND REMOTE ACCESS.

* STEP 1 - USING MY GMAIL ID.
 
* STEP 2 - STRONG USER ROOT PAASWORD.
 
* STEP 3- ADDING PAYMENT METHODS.

* STEP 4- ENTER OTHER NECESSARY FIELDS AND CREATE YOUR FREE TIER AWS ACCOUNT.

Now after creating aws account it is necessary to make is secure and though most of the services are covered under free tier it is generally advised to to enable billing and free tier alerts on as safe practice. Users must enable MFA ( Multi Factor Authentication) using services like Google Authenticator. Also after MFA most of the people jump directly to use aws services but it is recommended to create IAM user by:

* STEP 1 - SEARCH IAM ON CONSOLE.

* STEP 2 - ON LEFT SIDE GO TOWARDS USERS AND CREATE USERS.

* STEP 3 - TICK AWS MANAGEMENT CONSOLE ACCESS AND PROVIDE OR GENERATE PASSWORD.

* STEP 4 - IN POLICIES SELECT ADMINISTRATOR ACCESS THEN CREATE.

* STEP 5 - SAVE LOGIN CREDENTIALS AND IF POSSIBLE ADD MFA TO IT ALSO.

AFTER SUCCESSFUL CREATION OF MY AWS ACCOUNT THIS WAS MY DASHBOARD:

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/AWS%20Dashboard.png" width="800"/>
</p>

<p align="center"><em>Figure 2: My AWS Dashboard displaying health, cost, recent and other app bars.</em></p>

#### In the upcoming sections I would be explaining in detail about launching or running EC2 instances and conguring them as web server on cloud.

## EC2 WINDOWS INSTANCE


### FOLLOW THESE STEPS-



* Step 1: Search EC2 in the dashboard search box.

* Step 2: Then click on the launch instance button.

* Step 3: CHOOSE CONFIGURATION name as of your choice.

* Step 4: Select AMI as windows server 2019/2022 base.

* Step 5: Choose instance type as t2.micro.

* Step 6: This is a important step. Click on create new pair. Enter suitable name, choose type RSA and format as .pem.

* Step 7: Download the key ans store it in the safe place.

* Step 8: Under network settings allow RDP 3389 and allow HHTTP/HTTPS options available.

* Step 9: Choose storage as default or upon of your choice.

* Step 10: Press launch and wait.

NOTE: NEVER CREATE TWO EC2 INSTANCES AT THE SAME TIME, MAKE SURE TO DELETE THE FIRST ONE BEFORE CREATING THE SECOND ONE.

---


* AFTER THE CREATION OF WINDOWS EC2 INSTANCE AGAIN GO BACK TO EC2 DASHBOARD AND YOU MUST SEE YOUR INSTANCE AND THEN WAIT AND REFRESH UNTIL YOU SEE 3/3 CHECK PASSED, STATUS RUNNING AND A PUBLIC IPV4 ADDRESS ASSOCIATED WITH IT. REFER THESE IMAGES.

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/EC2%20Windows%20Instance.png" width="800"/>
</p>

<p align="center"><em>Figure 3: My EC2 instance section showing my newly created windows EC2 instances along with its IPV4 address and running status.</em></p>


### RDP CONNECTION 

THIS SECTION TOOK A LOT OF TIME IN TROUBLESHOOTING FOR ALMOST 4 HOURS AS I COULD NOT FIGURE OUT EXACT REASON WHAT IS CAUSING THE PROBLEMS. I TRIED AND LOOKED UPON VARIOUS SECURITY GROUP SETTINGS SUCH AS CHECKING INBOUND TCP 3389 FROM MY CURRENT IP AND MAKING SURE MY INSTANCES HAS PUBLIC IPV4 ADDRESS. I ALSO CHECKED EVERYTHING EVEN DELETED AND RE-CREATED MY WINDOWS INSTANCE BUT I COULD NOT FIND THE EXACT REASON. IT WAS THEN I GOT TO KNOW THAT MY COLLEGE WIFI HAS SOPHOS FIREWALL INSTALLED WHICH CAUSED THE BLOCKING OF MY TCP 3389 PORT WHICH IS USED BY REMOTE DESKTOP PROTOCOL. I THEN USED MY MOBILE DATA TO ACCESS IT AND IT WORKED PERFECTLY FINE. 


NOW FOLLOW THESE STEPS-
* Step 1: Go to EC2 Dashboard look for instances box and click on your instance.

* Step 2: Click connect in top panel.

* Step 3: Click on get password.

* Step 4: Upload .pem key which you have downloaded while creating instance.

* Step 5: It will decrypt the password automatically and then download the RDP file.

* Step 6: Open it and login. For the first time it will give warning but click on yes.

* Step 7: Enter username mostly it is Administrator.

* Step 8: Copy paste the password which you have recieved.

* Step 9: Click connect and you will enter inside your server.

* Step 10: Activities on servers does  not reflect in your main system.

### TOWARDS IIS SHOWCASING

Now, after entering the server we can configure it as a web server, go to your instance and copy-paste the IPV4 address in your main system browser. You must have got could not connect to server error. Actually, it takes different path to make this configuration. For simplicity, I have just tried to showcase the windows IIS page.

---

* Step 1: Using the same method of RDP connection of your server enter inside of it.

* Step 2: Now, go to search bar and type server manager.

* Step 3: A dashboard will be opened, now go towards add roles section.

* Step 4: Now click next, next and another next to let the default congurations as it is.

* Step 5: Set the WEB IIS from the menu and add required features.

* Step 6: Fnally click install and wait for 5 minutes.

* Step 7: Go back to your system and refresh the browser of your ipv4 address and your must see a page like shown below.


<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/Configuration%20of%20WIndows%20IIS%20Services.png" width="800"/>
</p>

<p align="center"><em>Figure 4: This is my system's browser where i have entered the IPV4 address of my EC2 instances and then IIS page appeared. Even if i turn my system off the page will continue to work as it is hosted from AWS server not my local system.</em></p>

---

#### This lab provided a strong practical understanding of launching, configuring, and accessing cloud-based virtual machines. It also introduced real-world troubleshooting scenarios, emphasizing the importance of network configurations, security rules, and environment-specific constraints while working in cloud infrastructure.


---

## EC2 LINUX INSTANCE

### FOLLOW THESE STEPS SIMILAR TO WINDOWS-


* Step 1: Search EC2 in the dashboard search box.

* Step 2: Then click on the launch instance button.


<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/EC2%20Linux%20Instance.png" width="800"/>
</p>

<p align="center"><em>Figure 5: Basic settings and conguration page before you can launch your linux instance. Must remember to allow port 22 which later can help you to connect to your instance.</em></p>



* Step 3: CHOOSE CONFIGURATION name as of your choice.

* Step 4: Select AMI as amazon linux 2023.

* Step 5: Choose instance type as t2.micro.

* Step 6: This is a important step. THIS TIME YOU DON'T NEED NEW KEY PAIR JUST USE THE KEY PAIR YOU USED FOR WINDOWS INSTANCE.

* Step 7: Allow SSH PORT 22 and source anywhere 0.0.0.0/0.

* Step 8: Under network settings allow HHTTP/HTTPS options available.

* Step 9: Choose storage as default or upon of your choice.

* Step 10: Press launch and wait.

NOTE: NEVER CREATE TWO EC2 INSTANCES AT THE SAME TIME, MAKE SURE TO DELETE THE FIRST ONE BEFORE CREATING THE SECOND.

Before moving towards next steps, copy-paste the public IPV4 address of your linux instance in another tab of your browser and make sure if using wifi that it SHOULD NOT block remote connections.

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/Linux%20SERVER%20inside.png" width="800"/>
</p>

<p align="center"><em>Figure 6: You can also see your newly newly created instance by going into instance diagnostics.</em></p>

---

### CONNECT USING SSH

#### The best and easiest method is to use Command Prompt(CMD) of your device. It is so because you don't need to download anything it is built-in your device and ready to use. Though it was recommended to me to use XSHELL but it is generally better when to handle multiple session and you want GUI. For beginners, you can try CMD first.

---

Moving towards next steps-

* Step 1: Open CMD of your device.

* Step 2: Now you have to locate the location of your keys.

* Step 3: By default, all your downloads must come to Downloads section of your device.
Run these commands to confirm.

* Step 4: TYPE cd Downloads press enter then type dir again press enter you must see yor downloaded key pair.

* Step 5: Copy paste your SSH connection from your ec2 instances by going to ssh clients tab.
It could start like this (ssh -i yourkey.....) .

* Step 6: A prompt will come Are you sure you wan to continue connecting?
Just press yes and enter.

* Step 7: The connection might get closed at this step.
Repeat the above steps and this time just your ssh -i... command and press enter.

* Step 8: A window will apper AMAZON LINUX 2023 and final line [ec2-user... ] which shows you are inside your linux server.

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/Entering%20Linux%20instances%20through%20terminal.png" width="800"/>
</p>

<p align="center"><em>Figure 7: This is how you you would be entering inside your linux server from your command prompt now you can try thse commands or directly jump to make this as a web server using APACHE.</em></p>

---


### IMPORTANT LINUX COMMANDS YOU CAN TRY 

* TO SEE YOUR CURRENT LOCATION: pwd

* TO SEE FILES AND FOLDERS INSIDE IT: ls

* TO GO INSIDE A FOLDER: cd folder_name

* TO GO ONE STEP BACK: cd ..

* FOR ROOT: cd /

* FOR HOME: cd -

* TO CREATE NEW FOLDER: mkdir folder_name

* TO CREATE A NEW FILE: touch file1.txt

* TO SEE INSIDE THE FILE: cat file1.txt

---


### RUNNING WEB SERVICE ON YOUR LINUX INSTANCE

Firstly, make sure your linux instance has public IPV4 address which it should have if you have followed right instructions. Now, copy-paste the the public IPV4 address of your instance in youur new tab of your browser and refresh for which it will show this site can't be reached.

##### After this follow these steps-

* Step 1: In security tab of your instance look for security group and add this rule-
TYPE - HTTP
PORT - 80
SOURCE - 0.0.0.0/0

* Step 2: Update your system:
sudo yum update -y

* Step 3: Install apache:
sudo yum install httpd -y

* Step 4: Start apache:
sudo systemctl start httpd

* Step 5: Auto enable it:
sudo systemctl enable httpd

* Step 6: Check status: IF IT SHOWS RUNNING YOU ARE DOING WELL !!
sudo systemctl status httpd

TILL THIS POINT YOUR WEB SERVER HAS STARTED WORKING AND IT WILL SHOW DEFAULT IT WORKS ! PAGE. NOW YOU CAN DISPLAY YOUR OWN MESSAGE ON YOUR SERVER USING THIS.

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/Linux%20APACHE%20SERVER%201.png" width="800"/>
</p>

<p align="center"><em>Figure 8: If you have followed right commands then you would see your apache default page showing It Works ! You can edit this message also..</em></p>

* Step 7: echo "Enter your message" | sudo tee /var/www/html/index.html
 
<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/CODE%20to%20configure%20APACHE.png" width="800"/>
</p>

<p align="center"><em>Figure 9: Code to configure your linux instance as a web server.</em></p>

REFRESH YOUR IPV4 BROWSER PAGE AND YOUR MESSAGE WILL APPEAR LIKE MINE. :)

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/Linux%20APACHE%20SERVER%202.png" width="800"/>
</p>

<p align="center"><em>Figure 10: After fully editing your your default page with your custom messsage you would see it. In my case I have written it in hindi for fun. Also even if I would have closed my laptop then this message would still be there.</em></p>

##### NOW DELETE YOUR LINUX INSTANCE AND MOVE ON TO YOUR UBUNTU INSTANCE.

---

## EC2 UBUNTU INSTANCE

### FOLLOW THESE STEPS SIMILAR TO WINDOWS AND LINUX AND LAUNCH UBUNTU INSTANCE-

* Step 1: Search EC2 in the dashboard search box.

* Step 2: Then click on the launch instance button.


<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/EC2%20Ubuntu%20Server.png" width="800"/>
</p>

<p align="center"><em>Figure 11: The instance page for your ubuntu server looks almost same of youur windows and linux server. Just select right network settings and you are good to proceed next.</em></p>


* Step 3: CHOOSE CONFIGURATION name as of your choice.

* Step 4: Select AMI as Ubuntu.

* Step 5: Choose instance type as t2.micro.

* Step 6: This is a important step. THIS TIME YOU DON'T NEED NEW KEY PAIR JUST USE THE KEY PAIR YOU USED FOR WINDOWS INSTANCE.

* Step 7: Allow SSH PORT 22 and 80 with source anywhere 0.0.0.0/0.

* Step 8: Under network settings allow HHTTP/HTTPS options available.

* Step 9: Choose storage as default or upon of your choice.

* Step 10: Press launch and wait.

---

### CONFIGURATION OF UBUNTU WEB SERVER

##### WE ARE GOING TO PROCEED DIRECTLY FROM CLOUDSHELL OF AWS FROM TOP CENTRE PART OF YOUR DASHBOARD TO CONNECT TO IT. 

* Step 1: Enter the SSH command or copy-paste it.
ssh -i yourkey.pem..... and then proceed.

* Step 2: You will be asked are you sure you want to continue cnnecting ?
Enter YES and proceed.

YOU MUST SEE WELCOME TO UBUNTU TYPE MESSAGE LIKE THIS.

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/Entering%20Ubuntu%20directly%20from%20cloudshell.png" width="800"/>
</p>

<p align="center"><em>Figure 12:DON'T FORGET TO FIRSTLY LOCATE YOUR KEY THEN TO ADD. After which your will a big message like this appears for you- WELCOME !!</em></p>

* Step 3: After successful login, update your system-
sudo apt update && sudo apt upgrade -y

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/APACHE%20Ubuntu%20configuration%20code%201.png" width="800"/>
</p>

<p align="center"><em>Figure 13: CONFIGURING UBUNTU SERVER.</em></p>

* Step 4: Install apache:
sudo apt install system -y

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/APACHE%20Ubuntu%20configuration%20code%202.png" width="800"/>
</p>

<p align="center"><em>Figure 14: MAKE SURE YOU ENTER CORRECT COMMANDS.</em></p>

* Step 5: Start apache and enable it -
sudo systemctl start apache2
sudo systemctl enable apache2

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/APACHE%20Ubuntu%20configuration%20code%203.png" width="800"/>
</p>

<p align="center"><em>Figure 15: FINALLY APACHE WORK WOULD HAVE BEEN DONE.</em></p>

YOUR DEFAULT APACHE PAGE WILL APPEAR LIKE THIS. 

---

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/APACHE%20ubuntu%20default%20page.png" width="800"/>
</p>

<p align="center"><em>Figure 16: This is your default apache page which we will change and display our simple custom message.</em></p>

---

### * Step 6: MOST IMPORTANT LAST STEP -

cd /var/www/html

* DELETE THE DEFAULT FILE -
sudo rm index.html

* CREATE NEW FILE -
sudo nano index.html

* NANO TEXT EDITOR WILL BE OPENED NOW WRITE LIKE THIS AND FOLOW THESE COMMANDS -

YOU NOW HAVE TO ENTER YOUR CUSTOM HTML MESSAGE- 

* TRY USING OTHER HTML TAGS TO PLAY ALONG .

DONE !!.

NOW do CTRL + 0 AND CTRL + X.

#### GO TO YOUR IPV4 ADDRESS AND REFRESH WINDOW AND SEE YOUR MESSAGE LIVE ON CLOUD.

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/PRACTICE_LAB/LAB_SCREENSHOTS/My%20message%20on%20ubuntu%20server.png" width="800"/>
</p>

<p align="center"><em>Figure 17: This was my message on my ubuntu server you can try yours too using html commands on nano editor.</em></p>

---


# KEY LEARNINGS


The lab sessions played a transformative role in shaping both my technical foundation and problem-solving mindset in cloud computing. Through hands-on interaction with cloud services, I developed a clear understanding of how virtual infrastructure is configured and managed in real-time environments. Working with different operating systems and executing commands at the system level enhanced my confidence in navigating cloud-based resources independently. More importantly, I learned how to approach errors logically, analyze configurations, and resolve issues through iterative debugging rather than relying solely on theoretical knowledge.

From a professional perspective, these sessions helped me move beyond basic concepts and develop a practical intuition for cloud workflows and system behavior. I understood the importance of precision in configuration, security awareness, and structured execution while working in a cloud environment. This phase also strengthened my ability to break down complex tasks into manageable steps and document them effectively. With this strong foundation and hands-on exposure, I am now well-prepared to move forward into building real-world solutions, as demonstrated in the upcoming minor project involving serverless architecture and automated workflows.
