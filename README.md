# Krishna Prasads level-1 report:

# Task 1 : Working with version control
In this task i learned about version control and its importance. Be it working with a team or solo project, relying on version control is a safe choice.
It helps to keep the track of the progress of the project and helps come back in time to correct any bugs or any issues that arised from past commits. For this task i used Git and GitHub to perform version control both locally and remote.

I used :
- `git init` - to initialize an empty repository locally 
- `git add` . - to stage changes
- `git commit` - to commit the changes
- `git diff` - to view the changes in the code
- `git clone` - to clone an existing repo
- `git status` - to check the status of staging and commiting
- `git log` - to see commit history
- `git branch` - to see and create branches
- `git checkout ` - to change or switch between branches
- `git merge` - to merge another branch to a branch(mainly done to main/master branch)
- `git remote add origin <repo-url>` to add remote
- `git push` - to push changes to remote repo
- `git stash` - to temporarily save changes
- `git stash list ` - lists all the saves
- `git stash apply` - to apply stash
  and many more commands.

  I understood the basic flow of branches and how they merge to the functional main branch to contribute to a new feature, further improving the website.

  when I explored the GitHub i could learn things much easily and quickly , everything was at fingertips , no need to write any commands , just click buttons to create new branch, go to pull request to merge the changes to another branch, to see logs you can click commits tab etc...

snippet:
![website](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/Screenshot%20(465).png?raw=true)

# Task 2: Database task - DynamoDB
In this task i learned about different **Database systems**. There are three main **Database systems** namely 1. SQL, MySQL, NoSQL.
All the three have their own advantages and disadvantages. 

**SQL:**  *Structured Query language* is a language used to communicate with relational database. It is used in querying and operating the database. ex: MySQL

**MySQL:** MySQL is a *relational database*(database consisting of related tables) in  which we use **SQL** to manage(insert, delete, etc..) the data present in the database and also the most popular in the market.

**No SQL:** *Not Only SQL* is a *non relational database* that doesnot use SQL, here the data is not stored in related tables as columns or rows but instead it stores as: 1) JSON like docs(MongoDB) 2) Key value pairs(DynamoDB) 3) Column data storage (Apache Cassandra) 4) Graph databases(Neo4j). This is more scalable because of its dynamic schema

The objective of this task was to use DynamoDB from AWS and creat aa simplw login system.
![website](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/Screenshot%20(480).png?raw=true)
![website](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/Screenshot%20(478).png?raw=true)
![website](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/Screenshot%20(533).png?raw=true)

- Here the new user information is saved in the database and while registering.
- The database saves the username, password and email as key value pairs.
- when you try to login with the already registered credentials you get a message called "Login Successsful" with a status code of 200
- If you enter wrong credentials you get to see "User not found message"
  
# Task 3: Create an application on EC2 instance
**EC2(Elastic Compute Cloud):** It is a service from the *Amazon Web Services* in which they give you access to virtual computer so that you can run your website or webapplication the internet accessible to ayone with the public ip. In your local machine you are the only person who can see and run the website or webapp. But with EC2, your application runs on a virtual machine in the Amazons data center where your code sits and runs on cloud giving access to the public.
Some important components of EC2:
- AMI(Amazon Machine Image): It contains the OS and software. for my task i used default Amazon Linux.
- Instance type: here you can select different instance types based on the scale of your project. i built a simple webapp so i used t3 micro which also comes under free tier. for larger porjects you can use t3 medium.
- Security groups: These are firewalls which controls the inbound and outbound traffic based on what security groups we set. For this task i allowed SSH, HTTP and HTTPS.

In this task  i learned how to create, configure and manage EC2. For this task i launched a simple temperature conversion app. I learned the basic commands of the CLI and installed httpd then cloned the git repository of the application, and then edited the inbound rules and allowed HTTP and HTTPS in the security groups and finally enabled and started the httpd. Once all this was done the application was up and running on the public ip.
![website](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/Screenshot%20(501).png?raw=true)
![website](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/Screenshot%20(502).png?raw=true)


# Task 4: AWS Cloudfront and S3 Buckets
**CloudFront** is the *CDN*(content delivery network) of *Amazon Web Services*. It delivers contents such as photos, videos, applications, etc... around the world with low latency. When a user user searches for a data for the first time CloudFront delivers the data from the origin(S3), once this happens it caches the data and then when another user else here searches for the same data the data is delivered the data is delivered instantly because it was chached already that is why it did not go to origin to find the data, this ensures low latency quick response.

**Amazon Simple Storage Service:** S3 is an object storage service , here we can store photos, videos, codes, PDFs,etc... In S3 we have to ceate a bucket with a unique name that serves as the container inside which the data resides. S3 can host static websites.

In this task i created an S3 bucket with an image of an island called Tahiti which was in a html file. In the CloudFront the I completed the required confifurations and set the created S3 bucket with static webpage as the origin. once the data is cached it is stored in edge locations in the world.You could apply Ddos portection. Invalidation removes files from the CDN cache so users get the updated version.
![website](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/Screenshot%20(536).png?raw=true)

# Task 5: OSI Model
**Open Systems Interconnections(OSI)** is a framework used to understand how different systems communicate between each other over a network(Ex: windows machine communication with Mac machine).It is divided into seven layers , each responsible for specific function in the process of data transmission , ranging from physical hardware connections to high-level application interactions.

The seven layers are :
| Sl No | Layer |
|-------|-------|
| 7 | Application|
| 6 | Presentation Layer|
| 5 | Session |
| 4 | Transport |
| 3 | Network |
| 2 | Data-Link |
| 1 | Physical Layer |

![website](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/OSI%20Model.drawio%20(1).png?raw=true)
![Website](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/ChatGPT_Image_Sep_15_2025_11_29_37_AM.webp?raw=true)

# Task 6: Kali Linux
Kali Linux is an open-source, Debian-based Linux distribution geared towards various information security tasks, such as Penetration Testing, Security Research, Computer Forensics and Reverse Engineering.
The obective of this task is to perform a penetreation testing on a virtual machine using Kali liux.
Firstly i installed virtual box which serves and a platform to run kali
