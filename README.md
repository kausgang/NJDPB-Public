## This is the public repository used in NJDPB Project.

Check out different branches for different work


Spring Boot Website Monitor - Comprehensive Guide

📌 Introduction

This project is a Spring Boot application designed to monitor website availability and SSL certificate validity. It checks whether a website is reachable and verifies the expiration date of its SSL certificate.

📖 Table of Contents

Project Setup

How It Works

Installation Guide

Configuration

Running the Application

Testing the Application

Extending the Project

🚀 1. Project Setup 

This project consists of:

Spring Boot Application (SpringWebsiteMonitorApplication.java)

Website Monitoring Service (WebsiteMonitor.java)

Unit Tests (WebsiteMonitorTest.java)

Maven Dependencies (pom.xml)

Configuration File (application.properties)

🛠️ 2. How It Works 

The application performs two main functions:

Website Availability Check: Sends an HTTP request to a specified URL and checks if it responds.

SSL Certificate Check: Retrieves the SSL certificate, extracts the expiration date, and calculates the remaining validity.

🖥️ 3. Installation Guide 

Prerequisites

Ensure you have the following installed:

Java 17 or later

Apache Maven

Spring Boot CLI (optional)

Git (optional)

Clone the Repository

git clone https://github.com/YOUR_USERNAME/NJDPB-Public.git
cd NJDPB-Public

Build the Project

mvn clean install

⚙️ 4. Configuration 

Update the application.properties file with your target website URL.

# application.properties
url=https://example.com

▶️ 5. Running the Application 

Start the Spring Boot Application

mvn spring-boot:run

Expected Output

URL is - https://example.com
HTTP Status Code: 200
SSL certificate is valid until Sat, 01 Jan 2025

✅ 6. Testing the Application 

To run unit tests:

mvn test

Sample Test Cases

testWebsiteReachability(): Ensures the website is reachable.

testSSLCertificate(): Checks SSL certificate validity.

📌 7. Extending the Project 

Possible Enhancements

✅ Email Notifications: Send alerts if SSL certificate is about to expire.
✅ Database Logging: Store monitoring results in a database.
✅ Multi-Site Monitoring: Support multiple URLs for monitoring.

📢 Conclusion

This guide provides all the necessary steps to install, configure, run, and test the Spring Boot Website Monitor. 🚀
