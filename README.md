CS 3338 Final Project - Group 4 - Landfill e-forms Application

Jira Project URL: https://calstatela-cs3338-spr25.atlassian.net/jira/your-work

**Team**
* Brian Becerra
* Jason Salazar
* Krystal Lo
* Mark Canseco

**Overview**
The LEF application will be a web-based application and a mobile application that allows users to submit and manage landfill-related forms electronically. The application will provide a user-friendly interface designed to streamline the process of submitting and managing forms.

The system comprises:

An Android Mobile Application: For field inspectors to collect data on-site.
A Web Application: For office staff to upload, audit, and store data in a centralized database, and generate reports.

**System Architecture**

The application follows this general workflow:

1.  **Data Capture:** Field inspectors use the Android Mobile Application to collect data, which is initially stored locally in an SQLite database on the device.
2.  **Data Synchronization:** The mobile application synchronizes the locally stored data with the central server via an API.
3.  **Central Data Storage:** The Spring Backend Server receives and stores the data in a Microsoft SQL Server database.
4.  **Data Access and Reporting:** Office staff use the Angular 4 Web Application to access, review, manage, and generate reports from the data stored in the central database.

**Features**

* **Mobile Application (Android):**
    * Data capture for various landfill-related forms.
    * Audit data capture.
    * Local data storage (SQLite) for offline functionality.
    * Data synchronization with the central server.
    * User login.
    * Data export to JSON.
    * Display of data to the user.
    * Processing data from the web application.
    * Notification of site completion status.

* **Web Application:**
    * Data management and storage.
    * Data review and auditing.
    * Report generation.
    * User interface for accessing and managing data.

**Technologies Used**

- **Mobile Application:**
    * Android
    * SQLite
    * Retrofit

- **Web Application:**
    * Angular 4
    * Java
    * Spring Framework (Spring Boot)
    * Gradle
    * HTML, CSS, JavaScript
    * SQL Server
