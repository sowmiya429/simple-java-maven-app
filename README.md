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

