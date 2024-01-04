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
go to dashboard-->manage jenkins--->tools
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/b9e20ed7-b0e4-4269-bcaa-7ab0a81599be)
add the location where the maven has installed
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/434b5959-e1e5-4a6c-84a8-6636be184f7a)
Create the new Freestyle project jenkins_maven11
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/c01d55b6-9d40-4ad0-a8d0-32caed8b96f0)
#Now you need to tell jenkins where the maven has located
configure Github
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/17e2f7d3-1bea-48be-a0d8-00f4437d3a3c)
Test the maven
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/9cf0bf7c-8e57-41d6-9492-41f289f5c66f)
now build 
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/1e31c6ae-3f0c-4cc9-874a-3ca05d7d9a38)
create post-build actions
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/a8af0b9e-71d9-4abf-aaaa-37f2badeb7f7)
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/16771331-2395-40bb-aced-349f5e8c6f01)
In this step create one more build step for creating package
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/bc5782af-eabf-4573-b576-6bda86b326d8)
Build now the package will create
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/103f8532-c3e2-4c6c-87f4-a939f826921e)
now the jar file has been created
<img width="848" alt="image" src="https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/1fc19200-bef2-4c69-8ae2-f348af4f50d0">
Last step is to run the jar file using below command
```
java -jar target/*.jar
```
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/be09a69b-c44d-4359-a444-1a44b883dc9d)
Now again buildnow
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/88bbe0fb-4a83-43b3-9bae-f4b0ecd16b7b)
result has comeup
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/f7e5eff7-5b2d-4c67-9cd9-eb37fdf39e2b)
Now create the artifact
![image](https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/61e7d8ce-a11a-4fbf-8515-d2559b59c4e4)
after the creating the artifact the link has been provided automatically
<img width="960" alt="image" src="https://github.com/sowmiya429/simple-java-maven-app/assets/80743760/16449e0d-c45b-4966-b07f-e1cb4587dc7b">
