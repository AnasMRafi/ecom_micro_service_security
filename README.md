# Keycloak Configuration & Testing Log

**Project:** E-Commerce Microservice Security

## 1. Keycloak Server Configuration

### 1.1. Configure Client (`ecom-client-angular`)
Set up the `ecom-client-angular` client for the frontend application.
*   **Client ID:** `ecom-client-agular`
*   **Client Authentication:** `Off` (Public Client) for Angular / `On` for Confidential access testing.
*   **Authentication Flow:** Standard Flow & Direct Access Grants (for Postman testing).
<img width="1512" height="904" alt="keycloak_client" src="https://github.com/user-attachments/assets/1fdcf10a-a525-4e55-8010-ed727c84c8e0" />


### 1.2. Create Roles
Defined the necessary roles for the application (e.g., `ADMIN`, `USER`).
<img width="1512" height="904" alt="keycloak_roles" src="https://github.com/user-attachments/assets/20f0282a-864d-4673-881b-a7857808f36d" />


### 1.3. Create Users
Created users and assigned them the appropriate roles.
<img width="1512" height="904" alt="keycloak_users" src="https://github.com/user-attachments/assets/40fabb65-a586-40fb-84e0-547d4251378c" />



---

## 2. Postman Testing

### 2.1. Get Token (Password Grant)
Obtaining an access token using the `password` grant type (Direct Access Grants).
<img width="1512" height="904" alt="postman_password_keycloak" src="https://github.com/user-attachments/assets/eed6f5ca-b6fb-4586-8d93-e4c1350f9ad4" />



### 2.2. Refresh Token
Using the refresh token to obtain a new access token.
<img width="1512" height="904" alt=" postman_refresh_token_keycloak" src="https://github.com/user-attachments/assets/275b3c03-25d9-4c75-b4db-3c5628453fc3" />


### 2.3. Get Token with Client Secret (Confidential Client)
*Note: This applies if Client Authentication is enabled.*
<img width="1512" height="904" alt="postman_client_secret_keycloak" src="https://github.com/user-attachments/assets/933db921-37ae-4dec-b790-63b344541707" />


### 2.4. Verify JWT Authentication
Testing the token verification.
<img width="1512" height="904" alt="postman_jwt_auth" src="https://github.com/user-attachments/assets/fb433142-9695-434a-ae67-e3dca52b7ed9" />


### 2.5. Access Protected Resource
Successfully accessing the `/products` endpoint using the Bearer token.
<img width="1512" height="904" alt="postman_jwt_products" src="https://github.com/user-attachments/assets/0fa86886-3fc2-4d7e-b9b7-280f7325ccc9" />
