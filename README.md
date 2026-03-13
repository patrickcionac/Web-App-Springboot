# Web-App-Springboot

Spring Boot Web Security Application
This project is a functional implementation of a web-based authentication system built using the Spring Boot framework and Spring Security. It demonstrates the fundamental concepts of securing a web application, including form-based login, session management, and access control.

Overview
The application provides a secure entry point where users must authenticate to access protected resources. It follows the standard Spring Security architecture to intercept requests, validate credentials, and manage the user lifecycle within the application.

Core Features
Form-Based Authentication: A custom login interface that captures user credentials.

Authorization Rules: Specific URL path protection ensuring that only authenticated users can access the home and greeting pages.

Session Management: Secure handling of user sessions, including a functional logout mechanism that invalidates the session and clears authentication data.

In-Memory User Store: Pre-configured user credentials used to demonstrate the authentication flow without requiring an external database.

Technical Stack
Java 17: The core programming language.

Spring Boot 3.x: The primary framework for application bootstrapping and configuration.

Spring Security: The security module used for authentication and authorization.

Thymeleaf: The server-side Java template engine used for rendering HTML views.

Gradle: The build automation tool used for dependency management and project lifecycle.

Project Structure
WebSecurityConfig.java: Contains the security filter chain, defining which paths are public and which require authentication.

MvcConfig.java: Configures the view controllers for the application, mapping URLs to Thymeleaf templates.

templates/: Contains the HTML views (login, home, hello) managed by Thymeleaf.
