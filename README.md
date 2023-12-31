# DevOps Training Prerequisites

This document provides step-by-step instructions to install the prerequisite software for the team training on Ubuntu.

## Table of Contents

- [Git](#git)
- [Java 17](#java-17)
- [Maven](#maven)
- [Jenkins](#jenkins)
- [Podman](#podman)

## Git

Git is a version control system that allows you to track changes in your codebase. Follow these instructions to install Git:

1. Open a terminal.
2. Run the following command to install Git:
   ```bash
   sudo apt update
   sudo apt install git
   ```
4. Verify the installation by running:
   
git --version


## Java 17

Java is a widely-used programming language. Follow these instructions to install Java 17:

1. Open a terminal.
2. Install Java 17:
    ```bash
   sudo apt update
   sudo apt install openjdk-17-jdk
   ```

3. Verify the installation by running:
    ```bash
   java -vesion 
   ```
## Maven

Maven is a build automation tool used primarily for Java projects. Follow these instructions to install Maven:

1. Open a terminal.
2. Run the following command to install Maven:
   ```bash
   sudo apt update
   sudo apt install maven
   ```
3. Verify the installation by running:
    ```bash
   mvn --version 
   ```

## Jenkins

Jenkins is an open-source automation server used for continuous integration and delivery. Follow these instructions to install Jenkins:

1. Open a terminal.
2. Run the following command to install Jenkins
    ```bash
   curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee /usr/share/keyrings/jenkins-keyring.asc > /dev/null
   
   echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] https://pkg.jenkins.io/debian-stable binary/ | sudo tee /etc/apt/sources.list.d/jenkins.list > /dev/null
   
   sudo apt-get update
   
   sudo apt-get install jenkins
   ```
3. Follow post-installation steps once installation is completed
4. copy key from */var/jenkins_home/secrets/initialAdminPassword*
5. To copy you can use following command
   ```bash
   sudo cat  /var/jenkins_home/secrets/initialAdminPassword
   ```
   **Note: Ensure to check the right path in your browser after installation**

![image](https://github.com/kodekollab/devops/assets/139070180/efb73b2c-9419-4c38-9a94-7bab7aaa19d9)

**Refer for more info :**

https://www.jenkins.io/doc/book/installing/linux/#debianubuntu

Verify Jenkins installation:

http://localhost:8080

login with credentials provided during setup

## Ansible

Ansible is a configuration management tool which offers an architecture that doesn’t require special software to be installed on nodes, using SSH to execute the automation tasks and YAML files to define provisioning details

1. Open a terminal.
2. Run the following command to install Podman
    ```bash
   sudo apt-get update
   sudo apt install ansible
   ```
3. Verify ansible installation
    ```bash
   ansible --version 
   ```

## Podman

Podman is a tool for managing containers. Follow these instructions to install Podman:

1. Open a terminal.
2. Run the following command to install Podman
    ```bash
   sudo apt-get update
   sudo apt-get -y install podman
   ```
3. Verify Podman installation
    ```bash
   podman --version 
   ```

That's it! You have successfully installed the prerequisite software for DevOps sessions.



