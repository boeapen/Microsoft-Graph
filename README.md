# Graph API Samples

Welcome to my repository of **Graph API** samples! This repository contains a collection of sample projects and code snippets for working with **Microsoft Graph API**, demonstrating various use cases such as user management, email integration, calendar events, and more.

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Authentication](#authentication)
- [Samples Overview](#samples-overview)
  - [User Management](#user-management)
  - [Calendar API](#calendar-api)
  - [Mail API](#mail-api)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The **Microsoft Graph API** provides a unified endpoint for accessing a wide range of data in Microsoft 365 services. These samples aim to help developers understand how to interact with the API for everyday tasks like retrieving user information, sending emails, working with calendar events, and more.

Feel free to explore and use these samples to get a hands-on experience with the Microsoft Graph API.

## Getting Started

To get started with the Graph API samples in this repository:

1. **Clone the repository:**

    ```bash
    git clone https://github.com/boeapen/Microsoft-Graph.git
    cd Microsoft-Graph
    ```

2. **Install dependencies:**

    Depending on the sample, install any necessary dependencies. For example, if a sample uses Node.js, run:

    ```bash
    npm install
    ```

3. **Set up the Microsoft Graph API:**

    - Create an app in [Azure Portal](https://portal.azure.com).
    - Register your application and note the `client_id`, `tenant_id`, and `client_secret` (if required).
    - Configure the necessary permissions (e.g., `User.Read`, `Mail.ReadWrite`).

4. **Configure your environment:**

    Set up your app’s configuration in the code (usually in `.env` or config files), providing the credentials (like `client_id`, `client_secret`, and `tenant_id`).

## Prerequisites

To use these samples, you need:

- A Microsoft 365 tenant (for development/testing)
- A registered app in the Azure AD portal
- Basic knowledge of JavaScript, Python, or C# (depending on the sample)
- Familiarity with OAuth2 authentication and Microsoft Graph API concepts

## Authentication

Microsoft Graph API uses **OAuth 2.0** for authentication. Each sample in this repository uses different authentication methods, such as:

- **Client Credentials** for app-only authentication
- **Authorization Code Flow** for user-based authentication

Please follow the appropriate authentication flow for your chosen sample and make sure you have the required permissions granted.

## Samples Overview

### User Management

This sample demonstrates how to:

- Retrieve user profile data (`GET /me` or `GET /users/{id}`)
- Create, update, or delete users (`POST /users`, `PATCH /users`, `DELETE /users`)

### Calendar API

This sample demonstrates how to:

- Get calendar events (`GET /me/events`)
- Create, update, and delete calendar events (`POST /me/events`, `PATCH /me/events`, `DELETE /me/events`)
- Handle event reminders and attendees

### Mail API

This sample demonstrates how to:

- Read, send, and delete messages (`GET /me/messages`, `POST /me/sendMail`, `DELETE /me/messages`)
- Access mail folders and move messages between folders

## Contributing

Contributions to this repository are welcome! If you have suggestions for new samples, improvements, or bug fixes, feel free to fork the repository and submit a pull request.

Please ensure that:

- Code follows the project's structure.
- You’ve tested your code changes.
- You’ve updated the documentation, if necessary.

## License

This repository is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more information.
