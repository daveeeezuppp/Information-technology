# Multi-Tier Architecture

## What Is a Two-Tier Architecture?

A two-tier architecture is an application design that separates an application into two main parts: the web/application tier and the database tier. These tiers communicate with each other to provide services to users.

## The Web/Application Tier

The web/application tier handles user requests and displays the application's interface through a web browser. In this mission, Nextcloud serves as the web application, allowing users to access and manage their files through a browser.

## The Database Tier

The database tier stores and manages persistent information, such as user accounts, file metadata, and application settings. MariaDB is used as the database for the Nextcloud application.

## Why Separate Them?

Separating the web application and database into two containers makes the system easier to manage, maintain, and troubleshoot. Each container has its own responsibility, and either service can be updated or configured independently. This separation also helps organize the system and makes it easier to scale in the future.
