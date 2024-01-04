# simple-java-maven-app

This repository is for the
[Build a Java app with Maven](https://jenkins.io/doc/tutorials/build-a-java-app-with-maven/)
tutorial in the [Jenkins User Documentation](https://jenkins.io/doc/).

The repository contains a simple Java application which outputs the string
"Hello world!" and is accompanied by a couple of unit tests to check that the
main application works as expected. The results of these tests are saved to a
JUnit XML report.

The `jenkins` directory contains an example of the `Jenkinsfile` (i.e. Pipeline)
you'll be creating yourself during the tutorial and the `scripts` subdirectory
contains a shell script with commands that are executed when Jenkins processes
the "Deliver" stage of your Pipeline.
#create an EC2 instance
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/2e444729-007e-421b-9091-692b28f80eac)
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/0e0c62b8-906c-4af9-97d5-bb76f9b9bab0)
Update the packages
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/a7ef2345-3cdd-40bd-9447-425005938b90)
Install java because maven was developed by Java
```
sudo apt install openjdk-11-jre -y
```
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/5a86dee2-2447-410f-ab8f-74dae00aa4dd)
```
sudo apt install maven -y
```
create a directory ws5 and clone git module
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/d9fcd96e-3753-457d-885d-4743472bc82f)
now compile 
```
mvn compile
```
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/0e6a0f59-fc7c-4851-ab0e-186ced7cc882)
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/634699ce-1d0d-4071-b192-2e68b608bb07)
after the compiling go to /targets/classes you can find the file "com" is created
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/06591f04-7678-43b4-878e-4e81f99f95ca)
Now create a package
```
mvn package
```
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/a877354f-23ee-486c-9ea4-01484025fb1d)
Now if you go and check in target directory you can find the "JAR FILE HAS BEEN CREATED"
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/f7583c70-0108-4eeb-bd2b-0944f942b4d1)
if you check in the TARGET file you can see the output
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/dc62b142-9239-4b2d-b966-ff024006a561)
Now it is the time to test 
```
mvn test
```
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/d40c75db-0643-41ff-b147-dc786b6c1b22)
Steps:
step1: clone github
step2: compile 
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/9982c8b0-d84e-4a7a-ac55-962e091e4b77)
```
curl -fsSL https://pkg.jenkins.io/debian/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins -y
```
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/f93c78da-2e98-4be9-b450-cf5ef9284b9d)
for initial password 
```
sudo cat /var/lib/jenkins/secrets/initialAdminPassword
```
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/79666d5a-71ea-478f-b3e7-32a3ce2b7348)
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/9400c0f1-f41e-4672-8dca-f0fb9729952e)
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/f0c52a17-1a7e-42d6-afb1-5079dccc64ee)
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/1da8c30d-ef6f-480c-af49-4dc2ee2b3d21)
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/26d098b8-93a6-4e32-880f-97dd0e3bf5e1)
want to connect to maven need plugins
#GO TO Manage jenkins---> plugin--->available plugin
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/ad3f6991-7635-40dd-9e8b-0b9012f24b26)
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/4f9bf6a2-219d-4cc1-a7c5-dc1a640d7f64)
#Now you need to tell jenkins where the maven has located
go to dashboard-->manage jenkins--->tools
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/b9e20ed7-b0e4-4269-bcaa-7ab0a81599be)
add the location where the maven has installed
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/434b5959-e1e5-4a6c-84a8-6636be184f7a)
Create the new Freestyle project jenkins_maven11
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/c01d55b6-9d40-4ad0-a8d0-32caed8b96f0)

