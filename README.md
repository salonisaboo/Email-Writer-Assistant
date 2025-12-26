# Email Writer Assistant

Email Writer Assistant is a browser-integrated tool designed to generate automated email replies directly within the Gmail interface.  
The system combines a Spring Boot backend service with a JavaScript content script to enable seamless, one-click reply generation.

---

## Project Overview

The Email Writer Assistant enhances productivity by allowing users to generate contextual email responses without leaving Gmail.  
It integrates directly into the Gmail UI and communicates with a backend service using RESTful APIs.

The project focuses on frontend–backend integration, secure request handling, and browser DOM manipulation.

---

## Features

- Automated email reply generation using backend APIs  
- Direct integration within the Gmail interface  
- One-click reply action via a custom Gmail toolbar button  
- Secure request handling for email content  
- Lightweight frontend logic using JavaScript content scripts  

---

## Tech Stack

### Backend
- Spring Boot  
- RESTful APIs  

### Frontend
- JavaScript  
- Gmail DOM Integration (Content Script)  

### Tools
- IntelliJ IDEA  
- Visual Studio Code  
- Postman  

---

## System Architecture

- Spring Boot backend exposes REST endpoints for reply generation  
- JavaScript content script injects UI elements into Gmail  
- Email content is extracted from the DOM and sent securely to the backend  
- Generated responses are returned and displayed within Gmail  

---

## Installation and Setup

### Prerequisites
- Java JDK 17 or higher  
- Node.js (for development utilities if required)  
- Google Chrome browser  

---

### Backend Setup
```bash
git clone https://github.com/salonisaboo/Email-Writer-Assistant
cd email-writer-assistant-backend
mvn clean install
mvn spring-boot:run
