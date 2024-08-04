# BoardgameListingWebApp

## Description

**Board Game Database Full-Stack Web Application.**
This web application displays lists of board games and their reviews. While anyone can view the board game lists and reviews, they are required to log in to add/ edit the board games and their reviews. The 'users' have the authority to add board games to the list and add reviews, and the 'managers' have the authority to edit/ delete the reviews on top of the authorities of users.  

## Technologies

- Java
- Spring Boot
- Amazon Web Services(AWS) EC2
- Thymeleaf
- Thymeleaf Fragments
- HTML5
- CSS
- JavaScript
- Spring MVC
- JDBC
- H2 Database Engine (In-memory)
- JUnit test framework
- Spring Security
- Twitter Bootstrap
- Maven

## Features

- Full-Stack Application
- UI components created with Thymeleaf and styled with Twitter Bootstrap
- Authentication and authorization using Spring Security
  - Authentication by allowing the users to authenticate with a username and password
  - Authorization by granting different permissions based on the roles (non-members, users, and managers)
- Different roles (non-members, users, and managers) with varying levels of permissions
  - Non-members only can see the boardgame lists and reviews
  - Users can add board games and write reviews
  - Managers can edit and delete the reviews
- Deployed the application on AWS EC2
- JUnit test framework for unit testing
- Spring MVC best practices to segregate views, controllers, and database packages
- JDBC for database connectivity and interaction
- CRUD (Create, Read, Update, Delete) operations for managing data in the database
- Schema.sql file to customize the schema and input initial data
- Thymeleaf Fragments to reduce redundancy of repeating HTML elements (head, footer, navigation)

## How to Run

1. Clone the repository
2. Open the project in your IDE of choice
3. Run the application
4. To use initial user data, use the following credentials.
  - username: bugs    |     password: bunny (user role)
  - username: daffy   |     password: duck  (manager role)
5. You can also sign-up as a new user and customize your role to play with the application! 😊
____________________________________________________________________________________________________________

# ✍️ Installation Process DevOps Project

## AWS - VPC 
## AWS Network Environment setup
EC2 > Security Groups > launch-wizard-2 > Edit inbound rules
  - Private
  - Isolated environment
  - Deployment will secure
  - [inbound rules](https://github.com/jaiswaladi246/DevOps_Shack_Ultimate_Pipeline_12_march/blob/main/PHASE-1/Screenshot%202024-03-13%20002123.png)

#### Create this all EC2 Instances

**EC2 > Number of instances - 3 > Ubuntu Server 22.4 > t2.medium > Configure storage 25 GB**
 - Master - EC2-1
    - Slave1 - EC2-2
    - Slave2 - EC2-3

 **EC2 > Number of instances - 2 > Ubuntu Server 22.4 > t2.medium > Configure storage 20 GB**
- SonarQube - EC2-5
- Nexus - EC2-6

 **EC2 > Number of instances - 1 > Ubuntu Server 22.4 > t2.large > Configure storage 30 GB**
- Jenkins - EC2-4

 **EC2 > Number of instances - 1 > Ubuntu Server 22.4 > t2.large > Configure storage 20 GB**
- For Monitoring - EC2-7
    - Prometheus
        - Blackbox-exporter
        - https://github.com/prometheus/blackbox_exporter
    - Grafana
 
## Downlaod Packeges use with script
```sh
vi 1.sh > Paste inside if have more installation pkg
chmod +x 1sh - Change permissions to executable 
./1.sh - execute run script
```
      
## Install Plugins in Jenkins for this Project
####  After Installation And configure inside | Jenkins > Tools
  - JDK - Eclipse Temurin installer
  - Maven Integration
  - Maven - Config File Provider
  - Maven - Pipeline Maven Integration
  - Sonar - SonarQube Scanner - This is tool
  - Sonar - sonarQube server
  - Docker
  - Docker Pipeline
  - Docker-Build-step
  - Kubernetes
  - Kubernetes CLI
  - Kubernetes Client API
  - Kubernetes Credentials
____________________________________________________________________________________________________________






  
