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
