# Ecommerce-Website

# Author
Mohith L M
## Introduction
E-commerce website repository! This project is designed to create a seamless online shopping experience. With an easy-to-navigate interface, users can browse, search, and purchase products effortlessly. For store owners, the admin panel simplifies managing inventory, orders, and customers. Built with modern web technologies, this project is scalable and customizable, ideal for developers aiming to create or improve their own e-commerce sites. 

## Details
Clone the repository.
Open the project in your IDE: IntelliJ IDEA (recommended) or Eclipse.
If using IntelliJ IDEA, ensure it recognizes the project as a Maven and Spring Boot project. Also, adjust the working directory for Spring Boot to find the views (web pages). Check Web Directories in IntelliJ IDEA for guidance.
Make sure you're in the JtProject directory.
Configure the database connection in the application.properties file 
Run the project by executing the main method in JtSpringProjectApplication.java.
Open http://localhost:8080/ in your browser.
If you've run the basedata.sql script on the database, log in as admin with the provided credentials (admin/123); otherwise, manually create an admin user in the database.
For normal user access, use the credentials (lisa/765).

## Database

MySQL or MariaDB serve as viable database options for this project. You can set up the database connection in the application.properties file by specifying the relevant values for the following properties: (it's advisable to avoid using the root username and choose another one instead)

If encountering the error java.lang.IllegalArgumentException: Could not resolve placeholder 'db.driver' in value "${db.driver}", it suggests adjusting the mysql-connector-java version in the pom.xml file to match your MySQL version. Additionally, ensure to reload your Maven project after making this change.

    db.url=jdbc:mysql://[ip address of db]:[port of db]/ecommjava?createDatabaseIfNotExist=true
    db.username=[username]
    db.password=[password, if any]

After resolving this issue, it's necessary to populate the database with some initial data. This can be accomplished by executing the basedata.sql script on the database. Instructions for running this script may vary depending on the tool you're using to access the database, so it's recommended to refer to online resources for guidance.

## Endpoints

http://localhost:8080/

http://localhost:8080/register

http://localhost:8080/admin/products

http://localhost:8080/admin/customers

http://localhost:8080/admin/categories

http://localhost:8080/admin/Dashboard

## Some reference links to have an idea about the concepts used

https://maven.apache.org/guides/index.html

https://docs.spring.io/spring-boot/docs/2.6.4/maven-plugin/reference/htmlsingle/

https://docs.spring.io/spring-boot/docs/2.6.4/maven-plugin/reference/htmlsingle/#build-image

https://docs.spring.io/spring-boot/docs/2.6.4/reference/htmlsingle/#web

https://spring.io/guides/gs/rest-service

https://spring.io/guides/gs/serving-web-content
