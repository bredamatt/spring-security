# REST API Security using SpringBoot and KeyCloak 
This is a repository to be used for testing various REST API Authentication and Authorization techniques based on KeyCloak.

## KeyCloak
Keycloak is an open source Identity and Access Management solution aimed at modern applications and services. It makes it easy to secure applications and services with little to no integration requried at the application source-code level. The main benefit of using KeyCloak is that users authenticate via Keycloak rather than individual apps. Apps no longer need to deal with login forms, storing users, or authenticating users. The downside is that KeyCloak is a relatively centralised solution, which leaves the environment prone to attacks that make authentication impossible unless redundancy is dealt with by clustering the instances securely.

### Information on KeyCloak
https://www.keycloak.org/documentation.html

### Information on KeyCloak clustering and installation procedure in detail
https://www.keycloak.org/2019/04/keycloak-cluster-setup.html
https://www.keycloak.org/docs/7.0/server_installation/

### Installing StandAlone KeyCloak server
1. Download the Server .zip file from: https://downloads.jboss.org/keycloak/7.0.1/keycloak-7.0.1.zip
2. Extract the contents using ```unzip keycloak-version.number.x.zip ```
3. ```cd``` into the server distribution's ```bin``` directory.
4. Execute ```./standalone.sh```
5. After the server 
boots, open ```http://localhost:8080/auth``` and enter the initial admin user and password. The admin user can create realms and users, in addition to register applications to be secured by KeyCloak. 
6. You can then login to http://localhost:8080/auth/admin/ with your username and password.

## Usage