# Krishna Prasad's level-1 report:

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
Firstly i installed virtual box which serves and a platform to run Kali, and then i installed Kali Linux from their website and ran it in the virtual box. After all the initial setup i performed the penetration testing.

**What is Penetration testing ?**
Penetration testing(Pentesting) is practice where ethical hackers attempt to identify vulnerabilities in a system before malicious hackers could find and exploit it. Pentest involves scanning networks, identifying open ports, Detecting running services and finding vulnerabilities. In this task we perform pentest using Nmap

**Nmap(Network mapper):** Nmap is an open-source network scanning tool used to discover devices, identify open ports, detect services and their versions, and gather information about operating systems on a network.

For this testing set the network adapter 1 attached to *Bridged Adapter*, by doing this the LAN/WiFi detects Kali as a real machine eventhough it is running on a virtual environment.

- Firstly I public IP address of the host windows device because i planned to do pentest on this device.
- I used ping to test of it the target device was in reach. here exchange of data packets confirms the connection.
- Then i used nmap to to look for ports , its state and services.
- Next i did service detection.
- Finally found out the OS and other info.
![Nmap](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/WhatsApp%20Image%202026-03-07%20at%2001.36.49%20(1).jpeg?raw=true)
![Nmap](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/WhatsApp%20Image%202026-03-07%20at%2001.36.49.jpeg?raw=true)

A shell is a command-line interface that allows users to interact with the operating system by entering commands. In Kali Linux, the Bash shell is commonly used to execute system commands and security tools. During this task, the shell was used to run the Nmap tool from the Kali Linux terminal to scan the target system and identify open ports and services running on the machine. The shell acts as an intermediary between the user and the operating system, enabling efficient control and execution of penetration testing tools.

# Task 7: Encryption techniques
Data Encrytion is the process of scrambling data from readable to unreadable format(cipher text) and parties with authrization can unscrable the data to read the data. This is necessary because it secures coinfidential piece of information to stay confidential on the internet , so no unauthorized party gets to read the data even if the data is retrieved through backdoor access(eg: servers). The data here could be anything like files, documents, messages , etc..

**Caesar Cipher:** The Caesar Cipher shifts each letter in the plaintext by a fixed number of positions in the alphabet. This method is simple but breaks easily with bruteforcing

**Vigenère Cipher:** The Vigenère cipher is an improvement over Caesar cipher. Instead of a fixed shift, it uses a keyword to determine the shift value for each letter.

**Substitution Cipher:** In substitution ciphers, each letter of the plaintext is replaced with another letter based on a predefined mapping.

We can broadly group data encryption methods into two categories:

**Symmetric Encryption:**

In these methods of Encryption we use a single key to encrypt plaintext and decrypt ciphertext, the private access to the key with the sender and the receiver.

Some common symmetric algorithms are: 
- AES(Advanced Encryption Standard)
- DES(Data Encryption Standard)
- TripleDES

**Asymmetric Encryption**

In asymmetric encryption, two keys are used: a public key and a private key. Separate keys are used for both the encryption and decryption processes:
- The public key, as the name suggests, is either publicly available or shared with authorized recipients.
- The corresponding private key is required to access data encrypted by the public key. The same public key will not work to decrypt the data in this technique.

Examples: RSA(Rivest Shamir Adleman), ECC(Elliptic Curve Cryptography)

For this task I created a simple chat application that used AES encryption algorithm. Here the AES uses symmetric encryption to encrypt the entered message there is a use of private key here. Here both server and client have the key. The client message is converted into bytes then encrypted using AES and then is sent to the server using socket and is decoded in the server side usig the private key.

![client.py](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/Screenshot%20(540).png?raw=true)
![server.py](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/Screenshot%20(541).png?raw=true)

[CODE](https://github.com/Krishna-Prasad31/encryption-)


# Task 8: IP Addressing and Web Scraping

The internet relies on various networking protocols and addressing mechanisms to enable communication between computers. One of the most important concepts in networking is IP addressing, which allows devices to be uniquely identified on a network.

An **IP address** is a 32-bit number. It uniquely identifies a host (computer or other device, such as a printer or router) on a TCP/IP network.

**TCP/IP Protocol**

It is the fundamental communication protocol used on the internet.

**TCP(Transmission Control Protocol)** 
- Ensures reliable connection
- It breaks data into smaller packets

**IP(Internet Protocol):**
- It is responsible for routing the packets to the correct destination

Together they ensure the data is correctly transported from client to server.

**Web Scraping:**

Web scraping is the automatic method of extracting huge amounts of data from websites. The data that we get is usually HTML , to make it easier to read and to list out the contents parsing of this HTML is done through a python library called as BeautifulSoup.

You can even scrap an entire website or specific data the user wants(Eg: scraping an amazon page for fitness wrist band).

Here the scraper i used was a python program. the program scrapes data from website and then it uses Beautiful soup to parse the HTML and then a CSV file is generated for better readability. The website i scraped was [Fake Python Job Listings](https://realpython.github.io/fake-jobs/)

![website](https://media.geeksforgeeks.org/wp-content/uploads/20251112161655543930/export_cdc1ce8d-afd8-4255-853d-85976a2c737b.png)

![website](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/Screenshot%20(527).png?raw=true)
![website](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/Screenshot%20(526).png?raw=true)

[Code](https://github.com/Krishna-Prasad31/web-scraper)

# Task 9: Socket.IO

Socket.IO is a library that enables low-latency, bidirectional and event-based communication between a client and a server.

In a normal scenario the communication between client and server happens where the client sends a request to the server and the server responds, once this cycle is completed the connection is closed. Imagine that we wanted to build a realtime chat application, in this case when the message is sent to the server, the messages stays in the server for the client on the other side to see, the client has to repeatedly send request to the server asking if he has got a message until he finally see the message. This method works but it is an overkill, this repeated sending of request is called *Polling*, if there are many clients and all of them start polling all at once , this creates a load on server , this can impact the server negatively.

One of the better solutions for this problem is to not closing the connection once a request-response cycle is completed, instead we send a updrade header to websocket message through HTTP to the server. When the upgrade of websockets is done correctly the termination of the connection is out of equation. hence a bi-directional connection is established. In a realtime chatting application this avoids polling beacuse the connection didnt cease, so load on the server is reduced this makes a better communication between multiple persons.

Socket.IO enables real-time communication in chat applications by establishing a persistent connection between client and server, allowing instant bidirectional message exchange. It initially connects using HTTP and upgrades to WebSocket when possible, ensuring low latency and reliable communication.

*Note: If WebSockets are not supported, Socket.IO automatically falls back to HTTP Long Polling*

![website](https://miro.medium.com/1*3JZEcCK-Qzafd0EVwBeXGQ.png)
![website](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/Screenshot%20(542).png?raw=true)
![Website](https://github.com/Krishna-Prasad31/MARVEL---level-1-report/blob/main/Screenshot%20(543).png?raw=true)
[Code](https://github.com/Krishna-Prasad31/Socket.Io-Realtime-Chat-Application/tree/master)
