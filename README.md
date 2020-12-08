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

Steps to do in jenkins 
----------------------
1.Create a maven job
2.git repo : https://github.com/rjshk013/simple-java-maven-app/
3.goals & options : clean install

If job is created under pipelineproject -configure pipeline section as below :

Definition : pipeline script from SCM
give git repo : https://github.com/rjshk013/simple-java-maven-app
Script Path :jenkins/Jenkinsfile (If jenkins file is inside jenkins folder,if it is present in root directory no need to give pathfor Jenkinsfile

Preconfiguration of jenkins:
--------------------------
tools : Maven,Docker must be installed (using install automatically option from jenkins global tool configuration)
