# Integration Testing and Code Documentation

In this final homework assignment, you will enhance your **REST API application** from [previous tasks](https://github.com/AM1007/goit-pythonweb-hw-10).

## Technical Task Description

Create Documentation with Sphinx

- **Use Sphinx to generate documentation for your application.** Add appropriate `docstrings` to essential functions and class methods in the core modules.

- **Unit Testing.** Write unit tests for your application’s repository modules.

- **Integration Testing.** Cover your application’s routes with integration tests using the `pytest` framework.

- **75% Test Coverage.** Achieve over 75% test coverage for your application. Use the [pytest-cov](https://pypi.org/project/pytest-cov/) package to monitor and ensure coverage.

- **Caching with Redis.** Implement a caching mechanism using Redis.Cache the current user during authentication so the `get_current_user` function retrieves the user from the cache instead of querying the database on every request.

- **Password Reset Mechanism.** Implement a password reset mechanism for the REST API application.
- **User Roles and Access.** Add role-based access control for users with roles such as "user" and "admin". Ensure only administrators can change their default avatar independently.

## Additional Tasks

- **Access and Refresh Tokens.** Implement application authorization using JWT with both an `access_token` and a `refresh_token`.

- **Cloud Deployment.** Deploy your application to a cloud service of your choice.
  Provide a link to the deployed application.

## General Requirements for the Assignment

**1. Code Documentation**

- All key functions and class methods must include appropriate `docstrings` to enable documentation generation with Sphinx.

**2. Testing**

- Test modules should be structured according to the application’s directory layout.
- Use `pytest` to write both unit and integration tests.
- Ensure at least 75% test coverage across the codebase, verified with [pytest-cov](https://pypi.org/project/pytest-cov/).

**3. Redis Caching**

- Configure Redis as the caching service for your application.
- When implementing user caching, ensure data security and relevance.

**4. Password Reset**

- Implement a secure password reset mechanism with confirmation via email or another method.

**5. Role Management**

- Introduce a user role system.
- Enforce access control for operations restricted to administrators.

**6. Storing Confidential Data**

- Store all sensitive information and configuration details in a .env file. Do not include confidential data directly in the codebase.

**7. Containerization**

- Use Docker Compose to manage all services and databases required for the application.

### Additional Requirements (for Extra Tasks)

**1. JWT Tokens**

- Implement a secure mechanism to refresh access tokens using a `refresh_token`.

**2. Cloud Deployment**

- Ensure the application functions correctly after deployment to your chosen cloud service.
- Submit a link to the working application.
