# Spring Boot REST CRUD

This project is the origin built with **Spring Boot** that demonstrates how to create a simple **REST API** performing **CRUD (Create, Read, Update, Delete)** operations. It focuses on building REST endpoints using **RestController**, connecting to a **MySQL database** using **Spring Data JPA**, and managing entities using standard HTTP methods.

## Features

- REST API with CRUD functionality
- REST API design practices
- Deepens learning of java core
- API testing using **Postman**

## Dependencies

The project uses the following main dependencies:

- **Spring Boot Starter Web** – for building REST APIs.
- **Spring Boot Starter Data JPA** – for database operations.
- **Spring Boot DevTools** – for automatic restarts during development.
- **MySQL Driver** – for MySQL database connectivity.

## MYSQL WORKBENCH

**SCRIPT**
```sql
CREATE DATABASE  IF NOT EXISTS `employee_directory`;
USE `employee_directory`;

--
-- Table structure for table `employee`
--

DROP TABLE IF EXISTS `employee`;

CREATE TABLE `employee` (
  `id` int NOT NULL AUTO_INCREMENT,
  `first_name` varchar(45) DEFAULT NULL,
  `last_name` varchar(45) DEFAULT NULL,
  `email` varchar(45) DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=1 DEFAULT CHARSET=latin1;

--
-- Data for table `employee`
--

INSERT INTO `employee` VALUES 
	(1,'Leslie','Andrews','leslie@luv2code.com'),
	(2,'Emma','Baumgarten','emma@luv2code.com'),
	(3,'Avani','Gupta','avani@luv2code.com'),
	(4,'Yuri','Petrov','yuri@luv2code.com'),
	(5,'Juan','Vega','juan@luv2code.com');
