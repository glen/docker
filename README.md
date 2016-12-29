# Docker Compose

Utilizing docker-compose to create 2 systems - a CentOS Web app and a MYSQL Database Server

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

Make changes to spring-servlet.xml for ensuring you are connecting to the correct IP of the MySQL server - obtain the ip of the machine using
```
docker-machine ip
```

### Prerequisites

You need Docker and some knowledge of Terminal

### Installing

Steps to get the system up and running

Create a docker image eTAAP-Dashboard

```
docker-compose up 
```

To force a re-build, you can

```
docker-compose up --build
```

The mysql container will start and expose port 3306. There will be a database dump using the SQL file into the MySQL container.
The eTAAP-Dashboard container will start Tomcat with 8080 port exposed.


## Built With

* [Maven](https://maven.apache.org/) - Dependency Management



## Authors

* **Glen** - *Initial work*


## License

This project is licensed under the MIT License

## Acknowledgments

* Gavin