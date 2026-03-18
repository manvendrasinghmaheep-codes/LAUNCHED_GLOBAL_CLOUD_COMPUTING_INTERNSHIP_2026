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


# KEY LEARNINGS

The lab sessions played a transformative role in shaping both my technical foundation and problem-solving mindset in cloud computing. Through hands-on interaction with cloud services, I developed a clear understanding of how virtual infrastructure is configured and managed in real-time environments. Working with different operating systems and executing commands at the system level enhanced my confidence in navigating cloud-based resources independently. More importantly, I learned how to approach errors logically, analyze configurations, and resolve issues through iterative debugging rather than relying solely on theoretical knowledge.

From a professional perspective, these sessions helped me move beyond basic concepts and develop a practical intuition for cloud workflows and system behavior. I understood the importance of precision in configuration, security awareness, and structured execution while working in a cloud environment. This phase also strengthened my ability to break down complex tasks into manageable steps and document them effectively. With this strong foundation and hands-on exposure, I am now well-prepared to move forward into building real-world solutions, as demonstrated in the upcoming minor project involving serverless architecture and automated workflows.
