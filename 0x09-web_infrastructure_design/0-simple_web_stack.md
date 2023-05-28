# Specifics About This Infrastructure

* What is a server?
A server is a computer program or device that provides a service to another computer program and its user, also known as the client.

* What is the role of the domain name?
A domain name is a unique identifier that helps users locate a website on the internet. It serves as the web address of a website and is used as part of the website's URL.
The role of a domain name is to provide a memorable and intuitive way for users to access a website.

* What type of DNS record www is in www.foobar.com?
A record.

* What is the role of the web server?
A web server is a software application that runs on a computer and is responsible for processing requests from clients and sending back responses over the internet.
The primary role of a web server is to host websites and web applications, and to serve web content to users who access them through web browsers or other client software.

* What is the role of the application server?
An application server is a software platform that provides an environment for running web applications and services.
It is responsible for managing the execution of application code, handling requests from clients, and returning responses back to the clients. The primary role of an application server is to support the development, deployment, and management of complex web applications.

* What is the role of the database?
A database is a collection of data that is organized in a structured way to facilitate efficient storage, retrieval, and modification of information.
The primary role of a database is to provide a reliable and efficient mechanism for storing and managing data.

* What is the server using to communicate with the computer of the user requesting the website?
TCP/IP protocol suite.

<br>

# Issues With This Infrastructure

* SPOF
multiple SPOF in this infrastructure; for example, if MySQL database server is down, the entire site would be down.

* Downtime when maintenance needed
When we need to run some maintenance checks on any component, the server has to be turned off. Since there's only one server, the website would be experiencing a downtime.

* Cannot scale if there's too much incoming traffic.
It would be hard to scale this infrastructure becauses one server contains the required components. The server can quickly run out of resources or slow down when it starts receiving a lot of requests.
