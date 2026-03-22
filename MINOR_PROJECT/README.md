# MINOR PROJECT: THE RISE OF SERVERLESS AUTOMATION

The minor project marked a turning point in my cloud computing journey, where theoretical knowledge transformed into a fully functional, real-world system. After building a strong foundation through lab sessions, this project challenged me to design and implement an automated, event-driven architecture using modern cloud technologies. It was not just about executing a task, but about understanding how large-scale systems operate seamlessly without constant human intervention.

In today’s fast-paced digital world, automation is no longer a luxury but a necessity. Traditional systems often rely on manual processes or continuously running servers, which not only increase operational costs but also reduce efficiency. This project introduced me to the concept of serverless computing, where resources are dynamically managed, and execution is triggered only when required. The idea of building a system that responds automatically to events—without maintaining servers—was both fascinating and powerful.

The core objective of this project was to create an intelligent image processing pipeline that automatically resizes images when they are uploaded to cloud storage. This seemingly simple task reflects a much larger concept used in real-world applications such as social media platforms, e-commerce websites, and content delivery systems. By leveraging event-driven architecture, I was able to connect multiple cloud services in a seamless workflow, where each component performed its role independently while contributing to a unified system.

This project also tested my ability to handle real-world challenges such as debugging errors, configuring permissions, and integrating multiple services. There were moments of failure, confusion, and repeated errors, but each obstacle contributed to a deeper understanding of cloud systems. The transition from initial failures to final success was not just technical growth, but a mindset shift toward persistence and structured problem-solving.

Ultimately, this project represents more than just a technical implementation—it reflects my ability to design scalable, automated solutions using cloud technologies. It served as a bridge between foundational learning and advanced application, preparing me for more complex projects ahead. This was the moment where I truly began to think like a cloud engineer, ready to build systems that are efficient, scalable, and future-ready.

---

# PROBLEM STATEMENT: THE CHAOS OF MANUAL PROCESSING

#### The objective of my minor probject is to design and implement a pipeline that automatically resizes an image whenever a new image is uploaded to an Amazon S3 bucket.

The system must use:
* Amazon S3

* AWS Lambda

* Amazon EventBridge

#### My task is to build a solution where:

* A user/server uploads an image into an S3 bucket.

* The upload event triggers a Lambda function.

* The Lambda function resizes the image (e.g., 1080x1080 or 50% reduction, anything can be done).

* The resized image is stored in a separate S3 bucket.

* Logs must be generated in CloudWatch.

 ### The Architecture Requirements are:

* #### S3 → EventBridge → Lambda

### The Functional Requirements are:

The system must:

* Accept JPG and PNG images only.

* Automatically resize images on upload.

* Store resized images in a different bucket or folder.

* Maintain original file naming with a prefix (e.g., resized_, processed_, thumbnail_).

* Log execution details in CloudWatch.

* Handle errors gracefully.

### IAM & Security Requirements are:

* Create a dedicated IAM Role for Lambda.

* Follow least privilege principle.

* No use of root credentials.

* Enable bucket versioning (recommended).

### The required deliverables are:

* Architecture Diagram (draw.io)

* Source Code (Lambda function)

##### Screenshots of:

* S3 buckets

* Lambda configuration

* EventBridge rule

* CloudWatch logs

* Before & After image comparison

* README document explaining architecture design, event flow, IAM permissions and challenges faced during this project.


#### THE PROJECT'S DEPTH OF EXPERTISE IN SERVICE INTEGRATION ALONG WITH SUCH CONSTAINTS MADE IT A WORTHWHILE PROJECT WHICH HELPED ME TO GAIN VALUABLE EXPERIENCE OF CLOUD SERVICES.


---


# ARCHITECTURE OVERVIEW: THE BLUEPRINT OF SCALABLE POWER

The architecture of this project follows a simple yet powerful event-driven model. The workflow begins when a user uploads an image to the source S3 bucket → this action generates an event → the event is captured and routed through EventBridge → which then triggers the Lambda function → the Lambda function processes the image using the Pillow library → resizes it into the required dimensions → and finally stores the processed image in the destination S3 bucket.

This loosely coupled architecture ensures that each service operates independently while contributing to a seamless pipeline. The absence of continuously running servers makes the system efficient, scalable, and cost-effective. The entire process is automated, requiring no manual intervention once deployed.

---

## AWS S3: THE VAULT OF INFINITE STORAGE

Amazon S3 (Simple Storage Service) is a highly scalable object storage service used to store and retrieve data from anywhere on the internet. In this project, S3 plays a critical role by acting as both the source and destination storage system. The original images are uploaded to one bucket, which triggers the processing workflow, while the resized images are stored in another bucket. Its durability, availability, and event notification capabilities make it ideal for building event-driven architectures.

## EVENTBRIDGE: THE PULSE OF REAL TIME TRIGGERS

Amazon EventBridge is a serverless event bus that enables real-time communication between different AWS services. In this project, it acts as the central routing mechanism that listens for events generated by the S3 bucket and forwards them to the Lambda function. This ensures a decoupled architecture where services interact through events rather than direct dependencies, improving scalability and flexibility.

## CLOUDWATCH: THE EYE OF ETERNAL MONITORING

Amazon CloudWatch is a monitoring and logging service that provides insights into system performance and application behavior. Throughout this project, CloudWatch played a crucial role in debugging errors and analyzing execution logs. By examining logs generated during each Lambda execution, I was able to identify issues, track failures, and refine the system until it worked flawlessly.

## AWS LAMBDA: THE SOUL OF SERVERLESS EXECUTION

AWS Lambda is a serverless compute service that allows code to run in response to events without provisioning or managing servers. In this project, Lambda acts as the processing engine that resizes images. It is triggered automatically when an event is received and executes the Python code using the Pillow library to transform the image before storing it in the destination bucket.

## IAM: THE SHIELD OF SECURE ACCESS

AWS Identity and Access Management (IAM) is responsible for controlling access to AWS resources. In this project, IAM roles and policies ensured that each service had the appropriate permissions to interact with others securely. Proper configuration of IAM was essential to allow Lambda to access S3, write logs to CloudWatch, and function correctly within a secure environment.

---

# WORKFLOW: THE PATH OF EVENT DRIVEN SYSTEM

The workflow of this project begins with a simple action—uploading an image to the source S3 bucket. However, behind this action lies a powerful chain of automated processes. As soon as the image is uploaded, the S3 bucket generates an event notification, signaling that a new object has been created.

This event is then captured by EventBridge, which acts as the routing system and forwards the event to the Lambda function. Once triggered, the Lambda function extracts the image from the source bucket and processes it using the Pillow library. The image is resized to predefined dimensions, ensuring consistency and optimization.

After processing, the resized image is stored in the destination S3 bucket with a modified filename. This entire sequence happens within seconds and without any manual intervention. The system operates in a fully automated, event-driven manner, demonstrating the true power of serverless architecture.

What makes this workflow remarkable is its efficiency and scalability. The system only runs when required, consumes minimal resources, and can handle multiple uploads simultaneously. This project effectively showcases how independent cloud services can collaborate to create a seamless, automated pipeline.

---

# IMPLEMENTATION: DEPLOYMENT OF SERVERLESS POWER 

### CREATING S3 BUCKETS

* Step 1: Go to amazon S3 dashboard. 

* Step 2: Click on create bucket. 

* Step 3: Bucket names of your original and resized should be globally unique.

* Step 4: Ensure the region of both of your buckets should be same along with lambda function.

* Step 5: Must enable the versioning.

##### It helps in keeping the multiple versions safe for use. The older files will not get deleted.

* Backup

* Accidental deletion recovery

* Audit

* Recovery

---

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MINOR_PROJECT/MINOR_SCREEENSHOTS/Bucket%20versioning%20ENABLED.png" width="800"/>
</p>

<p align="center"><em>Figure 1: After creating your original bucket you must ensure that it's versioning is enabled under properties tab. This prevents accidental overwrites and allows recovery of previous versions if needed.</em></p>

---


* Step 6: Keep the rest of the settings as default.

* Step 7:Click on create bucket.

* Step 8: Repeat the same process for second bucket.

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MINOR_PROJECT/MINOR_SCREEENSHOTS/S3%20Buckets.png" width="800"/>
</p>

<p align="center"><em>Figure 2: After successfully creating your both the buckets your dashboard will look like this.</em></p>

---

### EVENTBRIDGE CONFIGURATION

Firstly, we will enable eventbridge for s3:

* Open your original image bucket.

* Go to properties.

* Scroll down to event notifications.

* Enable 'Send notifications to Amazon EventBridge for all events in this bucket' ON .

##### THIS WILL ENSURE THAT WHENEVER THERE IS A NEW IMAGE UPLOADED IN S3 IT WILL SEND NOTIFICATIONS

---

### IAM ROLES 

#### ITS GOAL IS TO PROVIDE ACCESS TO SERVICES UPON REQUESTS.

If IAM Role is not provided then:

Lambda will try:

* GetObject from S3

AWS responds with:

* AccessDenied

Then CloudWatch error :

* AccessDeniedException

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MINOR_PROJECT/MINOR_SCREEENSHOTS/IAM%20Dashboard.png" width="800"/>
</p>

<p align="center"><em>Figure 2: This is my IAM Dashboard showing security recommendations, resources, users, roles and policies.</em></p>

---

* Step 1: Go to Identity and Access Manangement .

* Step 2: Choose create role from menu.

* Step 3: Select AWS service and choose lambda.

* Step 4: Attach policies -

-> Amazons3fullaccess.

-> Cloudwatchlogsfullaccess.

* Step 5 - Give role name.

* Step 6: Create role.

---

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MINOR_PROJECT/MINOR_SCREEENSHOTS/IAM%20Image%20Resizing%20role.png" width="800"/>
</p>

<p align="center"><em>Figure 2: Image resizing role.</em></p>

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MINOR_PROJECT/MINOR_SCREEENSHOTS/IAM%20Policy%201.png" width="800"/>
</p>

<p align="center"><em>Figure 2: p1.</em></p>

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MINOR_PROJECT/MINOR_SCREEENSHOTS/IAM%20Policy%202.png" width="800"/>
</p>

<p align="center"><em>Figure 2: p2.</em></p>

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MINOR_PROJECT/MINOR_SCREEENSHOTS/IAM%20Roles%20List.png" width="800"/>
</p>

<p align="center"><em>Figure 2: role.</em></p>

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MINOR_PROJECT/MINOR_SCREEENSHOTS/IAM%20policies%20List.png" width="800"/>
</p>

<p align="center"><em>Figure 2: policy.</em></p>


### LAMBDA FUNCTION

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MINOR_PROJECT/MINOR_SCREEENSHOTS/Lambda%20Dashboard.png" width="800"/>
</p>

<p align="center"><em>Figure 2: After successfully creating your both the buckets your dashboard will look like this.</em></p>


* Step 1: Go to AWS Lambda.

* Step 2: Click create function.

* Step 3: Give a suitable name.

* Step 4: Choose runtime as python 3.10 .

* Step 5: Choose architecture as x86_64 if it isn't set as default.

* Step 6: In permissions choose existing role.

* Step 7: Create function.

* Step 8: After creating the function go to configurations and look for general configurations.

* Step 9: Edit and set timeout to 30 seconds or more.

* Click save.


### ADDING LAYER

* Step 1: Go to AWS Lambda.

* Step 2: Click on your function.

* Step 3: Scroll down to layer section and click on add a layer.

* Step 4: Choose specify an ARN.

* Step 5: Copy-paste the arn of according to your region and settings.

* Step 6: Then add and save .


### CREATING EVENTBRIDGE RULE

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MINOR_PROJECT/MINOR_SCREEENSHOTS/EventBridge%20Dashboard.png" width="800"/>
</p>

<p align="center"><em>Figure 2: EventBridge Dashboard showing resources, metrices along with created rules and groups.</em></p>

---

* Step 1: Go to amazon EventBridge.

* Step 2: Click rules and press create rule.

* Step 3: Give it a suitable name.

* Step 4: Now under event source, choose service as s3 and event type as object created.

* Step 5: Specify the name as your original bucket name.

* Step 6: In targets tab, choose target as lambda function and choose your lambda function.

* Step 7: Create rule.

---

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MINOR_PROJECT/MINOR_SCREEENSHOTS/Default%20EventBus.png" width="800"/>
</p>

<p align="center"><em>Figure 2: This is the default EventBus page.</em></p>

---

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MINOR_PROJECT/MINOR_SCREEENSHOTS/Target%20to%20lambda.png" width="800"/>
</p>

<p align="center"><em>Figure 2: This is important trigger page of my event which show target to lambda function.</em></p>

---

<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MINOR_PROJECT/MINOR_SCREEENSHOTS/Trigger%20Event%20Pattern.png" width="800"/>
</p>

<p align="center"><em>Figure 2: This is important event pattern section. The rule filters events where the source is Amazon S3 and the detail type is Object Created. When the condition matches, the event triggers the Lambda function which processes the uploaded image.”</em></p>

#### EVENT PATTERN -

 {
 
  "source": ["aws.s3"],
  
  "detail-type": ["Object Created"],
  
  "detail": {
  
    "bucket": {
    
      "name": ["manvendra-original"]
      
    }
    
  }
  
}


##### MEANING- 

* SOURCE: IT ONLY ALLOWS S3 SOURCE.

* RESTRICTION: BUT IN DETAIL TYPE WE RESTRICTED THAT ONLY OBJECT CREATION WILL BE CONSIDERED.

* NAMING: IT ALLOWS ONLY MY ORIGINAL BUCKET MODIFICATION TRIGGERS.

* IF ANY CONDITION FAIL TRIGGER WILL NOT HAPPEN.


---


<p align="center">
  <img src="https://github.com/manvendrasinghmaheep-codes/LAUNCHED_GLOBAL_CLOUD_COMPUTING_INTERNSHIP_2026/blob/main/MINOR_PROJECT/MINOR_SCREEENSHOTS/Rules%20Section.png" width="800"/>
</p>

<p align="center"><em>Figure 2: The default EventBus successfully shows enabled status to my event.</em></p>


---


## FINAL OUTPUT: THE TRIUMPH OF CLOUD

## CODE: THE LOGIC BEHIND THE LEGEND

* Step 1: Go to AWS Lambda.

* Step 2:Choose your resizing function and choose code tab.

* Step 3: Scroll down a editor will come and remove older code and write your own code.

* Step 4: After completing it click on deploy.

* Step 5: Wait for green check tick tox appearing.


---


# ERRORS: THE BATTLE AGAINST BUGS

The journey of this project was far from smooth, as it involved multiple challenges and unexpected errors that tested both my patience and problem-solving abilities. From initial configuration issues to runtime errors, each stage presented a new obstacle. One of the most recurring issues was related to event structures, where incorrect configurations led to errors such as missing keys in the event object. Additionally, permission-related problems in IAM caused failures in accessing S3 resources, highlighting the importance of precise role configuration.

Another major challenge was debugging Lambda execution failures using CloudWatch logs. At times, the function would execute successfully during testing but fail during actual S3 uploads due to differences in event triggers. These inconsistencies required careful analysis of logs, step-by-step verification, and repeated testing. There were multiple failed attempts—each one bringing frustration—but also deeper understanding.

What truly defined this phase was persistence. Instead of giving up, I approached each error as a learning opportunity. By systematically identifying the root cause, applying fixes, and retesting the system, I was eventually able to resolve all issues. The final success, after numerous failures, was not just a technical achievement but a testament to resilience and continuous learning in cloud engineering.

---

# CONCLUSION: THE DAWN OF CLOUD ENGINEER

The completion of this minor project marks a significant milestone in my journey toward becoming a cloud engineer. What started as a learning exercise evolved into a fully functional, event-driven system that demonstrated the power of serverless architecture. This project not only strengthened my technical understanding but also reshaped my approach to problem-solving and system design.

Through this experience, I gained practical insights into how modern cloud applications are built using loosely coupled services that communicate through events. The ability to design a system that automatically responds to user actions without manual intervention highlighted the efficiency and scalability of cloud computing. Concepts such as automation, event-driven workflows, and serverless execution are no longer just theoretical ideas for me—they are tools I have successfully implemented in a real-world scenario.

Beyond technical skills, this project also played a crucial role in developing my mindset. Facing multiple failures and debugging complex issues taught me the importance of patience, persistence, and structured thinking. I learned that errors are not obstacles but stepping stones toward mastery. Each challenge pushed me to explore deeper, understand better, and improve continuously.

This project serves as a bridge between foundational learning and advanced application. It has given me the confidence to tackle more complex systems and explore deeper aspects of cloud computing. The successful implementation of this automated pipeline proves that I am ready to move forward into building more sophisticated solutions.

As I transition into the major project, I carry forward not only the technical knowledge but also the confidence and experience gained from this journey. This marks the beginning of a new phase—one where I am no longer just learning cloud computing, but actively building and innovating within it. The rise of serverless automation is not just a project—it is the foundation of my path toward becoming a skilled cloud engineer.

---

