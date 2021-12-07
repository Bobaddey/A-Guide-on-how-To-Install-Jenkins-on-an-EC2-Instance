# A-Guide-on-how-To-Install-Jenkins-on-an-EC2-Instance

https://faun.pub/a-guide-on-how-to-install-jenkins-on-an-ec2-instance-ab9f17af7efa
![image](https://user-images.githubusercontent.com/60587384/145048143-c8137134-611d-4536-bf42-5a5aabd48afa.png)

Jenkins is an open-source automation server. It helps automate the parts of software development related to building, testing, and deploying, facilitating continuous integration and continuous delivery.

# What You will Need:

* An AWS Account
* Security group with port 8080 opened
* Java SDK 11
* Jenkins installer
* PUttY App (This will be used to connect to our Instance)
* An Internet connection
* And my Guide (lol)

# Setting up an EC2 Instance

* Login to your AWS account
* Search for EC2 in the search pane
* Go to “Instances”
* At the top right corner, click on ‘Launch Instance”
* Leave configurations as default till you get to the Tag section, you can type in Name: Jenkins_Server
* Next is the security group, remember this server should be accessible over the internet and port 8080 should also be accessible. By default, port 22 is included in our security group which allows access over the internet, but to allow access to port 8080,

Click on “Add rule” -> Set Protocol to TCP -> Set Port to 8080
* Then Review and Launch Instance
* You can Download existing or Create a new key pair if you don’t have one already. This will be used to SSH (i.e Connect) into our Instance.
