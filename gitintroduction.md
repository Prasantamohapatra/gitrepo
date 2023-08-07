# Installation and configuration of Git 

## I will be defining step by step instructions to configure git on the localhost

## Step 1 - Installation of git in Ubuntu 
```
sudo apt install git
```
## Runniing this command will show the below results 
![Alt text](image.png)

## To confirm that the Git is installed you can check with the bewlo command for verification
## Step2- Git installation status check
```
git --version
```
## This will show the below Result if same shows then it confirms that git installed

![Alt text](image-1.png)

## Step3 - Create a Dir to and switch into that 

```
mkdir gitrepo
```

## Step4- Switch to dir gitrepo
```
cd gitrepo
```
![Alt text](image-2.png)
## Step4- Configure the user name and usermain of Github inorder to intigrate with GitHub

```
git config --global user.name Prasantamohapatra
```
```
git config --global user.email prasantamohapatra568@gmail.com
```
![Alt text](image-3.png)

## Step5 - Check if the configuration done or not with below command
```git config --list
```
![Alt text](image-4.png)

## step6 - Innitialize the an git  repo to get started with git process
```git init
```
![Alt text](image-5.png)


## Step7 -- Generate SSH key for gitHub intigration

```ssh-keygen
```

![Alt text](image-6.png)

## Step 8 - Copy the ssh key following below command

```cat/home/ubuntu/.ssh/id_rsa.pub 
```
![Alt text](image-1.png)
## Step 9- Go to GitHub Settings and select SSH and GPG Keys and paste in side SSH key section.

![Alt text](image-2.png)

![Alt text](image-3.png)

## Step10- Create a new repo in GitHub

![Alt text](image-6.png)

## Step11 - Copy The SSH link 

![Alt text](image-5.png)
## Step12- Clone The repo to  the system

```
git clone git@github.com:Prasantamohapatra/GITDEMO.git
```
![Alt text](image-7.png)

## Step13 - Get into the DIR or create one and make changes 
```
echo "Hello World" > file1.txt
```
![Alt text](image-8.png)

## Step14 - Then move the changes to staging area by and check if done or not using the below commands

```
git add file1.txt
```


![Alt text](image-9.png)

```
git status
```

## Step15- Then Commit the changes to local repo 
```
git commit -m "added new file"
```
![Alt text](image-10.png)

## Step16 - Then Push the changes to main branch 

```
git push -u origin main
```

![Alt text](image-11.png)

## Step17 - Then refresh the git hub link to see the  changes in GitHub 

![Alt text](image-12.png)

# Congratulations you have sucessfully intigrated EC2 machine with GitHub