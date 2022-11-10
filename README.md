

![alt text](https://github.com/antkaynak/Keyist-Ecommerce/blob/master/screen_shots/detail.png)

![alt text](https://github.com/antkaynak/Keyist-Ecommerce/blob/master/screen_shots/cart.png)

![alt text](https://github.com/antkaynak/Keyist-Ecommerce/blob/master/screen_shots/browse.png)

![alt text](https://github.com/antkaynak/Keyist-Ecommerce/blob/master/screen_shots/orders.png)


## Getting Started
This project is a simple e-commerce website powered by Angular 10 on the frontend and Spring Boot for the backend.
<br>
For the full stack list please visit "Built With" section below.

Ecommerce is a complex business. It involves many edge cases and a solid system architecture. This project is simply a demo demonstrating basic features which is only the tip of an iceberg. This project might ( and certainly does ) have bugs, vulnerabilities or some other types of issues. So, contributions are always welcome :)

The demo is under free hosting, so it may require a bit of a patience :)

## Updated
This project is upgraded to Java 11, Spring Boot 2.3.3 and Angular 10+ and some new features added!

A docker-compose.yml added for you to bootstrap all of the aplication instances in one command!

## About This Project

* You can browse items or select an item from the showcase and preview.
* Browse section remembers your list choice, so even if you leave the page, when you come back you do not need to fetch products again.
* Your cart is saved on the database so you can login from different sources and still be able to use your cart.
* You can use discount coupons!
* You can store your information for faster purchase.
* You can view your orders and change your account settings.
* You can request a password forgot request and use the token in your mail.
* You can search items.


### Disclaimer
This is a fully functional demo site and may have security vulnerabilities as user data is not encrypted with SSL.
<br>
The provided codes are not ready for production and should only be used for education purposes.

### Prerequisites

What things you need to install

```
Angular CLI is recommended.
You need Tomcat server 8 or above installed or you can use embedded spring boot tomcat jar.
Locally installed MySQL or a MySQL server.
Compatible IDE, Intellij IDEA recommended for this project.

```

If you want to run the Dockerized version keep in mind that you must install Docker.
Also please note that booting up with docker-compose might take approx. 10-30min depending on your internet connection. After the initial setup, all other subsequent docker-compose commands will run much faster due to caching.

### Installing

The codes are split into 3 sections. 

frontend - Angular 10 ,

resource_server - Spring Boot Backend ,

authorization_server - A Spring Boot OAuth2 Authorization server.


To run the application fill the lines in resource server and authorization server application.properties as well as frontend application service urls.


For MySQL Database 

```
SQL script can be found in the sql folder.
script.sql contains both the basic user info and the tables for the oauth2 implementation.

```

For Tomcat Application Server

```
Use Tomcat 8.5.23 or above and compile to generate WAR file.
If you want you can use Spring Boot embedded tomcat JAR file and host it.
Keep in mind that both authorization and backend server's pom.xml is configured to compile a jar file.

```

For Undertow Application Server

```
This project uses undertow as default.
Keep in mind that both authorization and backend server's pom.xml is configured to compile a jar file.

```

This project uses Java Mail to create an embedded SMTP server. 
<br>
You can configure your own settings in the yaml file depending on your email provider or you can disable Java Mail altogether.
<br>

For Docker

```
In the root folder run the following command

docker-compose up

If you want to use development versions of the Dockerfiles, you need to setup docker-compose-yml to build using Dockerfile.dev.



