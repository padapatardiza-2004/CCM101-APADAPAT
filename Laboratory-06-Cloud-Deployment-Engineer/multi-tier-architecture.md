# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A Two-Tier Architecture divides an application into two connected parts: the Web/Application Tier and the Database Tier. Each tier performs a different responsibility, allowing the application to process user requests while keeping its stored information in a separate database system.

## The Web/Application Tier

The Web/Application Tier is the part that users interact with when accessing the application. It receives HTTP requests, processes application activities, and presents the user interface. In this deployment, Nextcloud serves this role.

## The Database Tier

The Database Tier handles the storage and management of information required by the application. It keeps persistent data such as application records and user-related information. In this deployment, MariaDB provides the database service for Nextcloud.

## Why Separate Them?

Using two separate containers keeps the application and database functions independent from each other. The web container can handle requests while the database container focuses on storing information, making the system easier to maintain and troubleshoot. Separating the two also allows each component to be managed without placing both functions inside one container.
