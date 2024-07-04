---
description: 'REPO: https://github.com/caleberi/shortify'
---

# Shortify

Shorifty is a URL shortener API developed on the Deno platform using TypeScript. It provides a simple and efficient way to convert long URLs into short, custom URLs. Additionally, users can link their custom domains to the URL shortener, making it a versatile tool for personal or business use.

#### Key Features:

* **Custom URL Shortening**: Easily create short URLs from long URLs for easy sharing and management.
* **User Authentication**: Secure user signup, login, and profile management to ensure that all created short links are associated with user profiles.
* **Custom Domain Support**: Allows users to connect their custom domains, serving as the base for all short links.
* **Statistics Tracking**: Provides detailed statistics for each short URL, enabling users to track the performance and usage of their links.

#### Technologies Used:

* **Deno**: A modern runtime for JavaScript and TypeScript that is secure and easy to use.
* **TypeScript**: A strongly typed programming language that builds on JavaScript, providing better tooling and error checking.

#### API Endpoints:

* **User Endpoints**:
  * `POST /users/signup`: Create a user profile to associate with all shortened links.
  * `GET /users/me`: Retrieve user profile information using the provided authentication token.
  * `POST /users/login`: Log in to a user account and retrieve an authentication token.
* **Short URL Endpoints**:
  * `POST /urls`: Create a new short URL.
  * `GET /urls/:code`: Retrieve the original long URL associated with a given short URL code.
  * `GET /urls/stats/:code`: Retrieve usage statistics for a specific short URL code.

#### Contribution Guidelines:

To contribute to Shorifty, follow these steps:

1. Fork the repository on GitHub.
2. Clone the forked repository to your local machine.
3. Install Deno on your machine.
4. Navigate to the project directory in your terminal.
5. Run `deno run --allow-net --allow-write --allow-read app.ts` to start the server.
6. Make your desired changes and commit them.
7. Push your changes to your forked repository.
8. Create a pull request to the main repository.

#### License:

Shorifty is licensed under the MIT License, making it free and open-source for anyone to use, modify, and distribute.
