# Docker Compose

Utilizing docker-compose to create 2 systems - a CentOS Web app and a MYSQL Database Server

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

You need Docker and some knowledge of Terminal

### Installing

Steps to get the system up and running

Create a docker image eTAAP-Dashboard

```
docker build -t eTAAP-Dashboard .
```

Once the web image is built, you can start docker-compose

```
docker-compose up
```

The mysql container will start and expose port 3306. There will be a database dump using the SQL file into the MySQL container.
The eTAAP-Dashboard container will start Tomcat with 8080 port exposed.

```
docker run -p 8080:8080 -it -d etaap_web
```

## Built With

* [Maven](https://maven.apache.org/) - Dependency Management



## Authors

* **Glen** - *Initial work*


## License

This project is licensed under the MIT License

## Acknowledgments

* Gavin