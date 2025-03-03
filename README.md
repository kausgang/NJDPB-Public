## Website Healthcheck

Java Springboot project to check website health


# Spring Boot Website Monitor - Comprehensive Guide

## 📌 Introduction

This project is a **Spring Boot** application designed to monitor website availability and SSL certificate validity. It checks whether a website is reachable and verifies the expiration date of its SSL certificate.

## 📖 Table of Contents

1. [Project Setup](#setup)
2. [How It Works](#how-it-works)
3. [Installation Guide](#installation-guide)
4. [Configuration](#configuration)
5. [Running the Application](#running-the-application)
6. [Testing the Application](#testing-the-application)
7. [Extending the Project](#extending-the-project)

---

## 🚀 1. Project Setup&#x20;

This project consists of:

- **Spring Boot Application** (`SpringWebsiteMonitorApplication.java`)
- **Website Monitoring Service** (`WebsiteMonitor.java`)
- **Unit Tests** (`WebsiteMonitorTest.java`)
- **Maven Dependencies** (`pom.xml`)
- **Configuration File** (`application.properties`)

---

## 🛠️ 2. How It Works&#x20;

The application performs two main functions:

1. **Website Availability Check**: Sends an HTTP request to a specified URL and checks if it responds.
2. **SSL Certificate Check**: Retrieves the SSL certificate, extracts the expiration date, and calculates the remaining validity.

---

## 🖥️ 3. Installation Guide&#x20;

### Prerequisites

Ensure you have the following installed:

- **Java 17** or later
- **Apache Maven**
- **Spring Boot CLI** (optional)
- **Git** (optional)

### Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/NJDPB-Public.git
cd NJDPB-Public
```

### Build the Project

```bash
mvn clean install
```

---

## ⚙️ 4. Configuration&#x20;

Update the `application.properties` file with your target website URL.

```properties
# application.properties
url=https://example.com
```

---

## ▶️ 5. Running the Application&#x20;

### Start the Spring Boot Application

```bash
mvn spring-boot:run
```

### Expected Output

```text
URL is - https://example.com
HTTP Status Code: 200
SSL certificate is valid until Sat, 01 Jan 2025
```

---

## ✅ 6. Testing the Application&#x20;

To run unit tests:

```bash
mvn test
```

### Sample Test Cases

- `testWebsiteReachability()`: Ensures the website is reachable.
- `testSSLCertificate()`: Checks SSL certificate validity.

---

## 📌 7. Extending the Project&#x20;

### Possible Enhancements

✅ **Email Notifications**: Send alerts if SSL certificate is about to expire. ✅ **Database Logging**: Store monitoring results in a database. ✅ **Multi-Site Monitoring**: Support multiple URLs for monitoring.

---

## 📢 Conclusion

This guide provides all the necessary steps to **install, configure, run, and test** the Spring Boot Website Monitor. 🚀

Would you like to add more features or automate deployment? Let me know!

