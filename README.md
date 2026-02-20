# API Documentation for Snippets Endpoint

## Overview
This documentation provides comprehensive information about the Snippets API, covering all CRUD operations.

### Snippets Endpoint
- **Base URL**: `/api/snippets`

### Authentication
- All endpoints require JWT token-based authentication.
- Include the token in the `Authorization` header as follows:
  ```
  Authorization: Bearer <your_token>
  ```

### CRUD Operations

#### 1. Create a Snippet
- **Method**: `POST`
- **URL**: `/api/snippets`
- **Request Body**:
  ```json
  {
      "title": "Snippet Title",
      "code": "print('Hello, World!')",
      "language": "Python"
  }
  ```
- **Response**:
  - **201 Created**
  ```json
  {
      "id": 1,
      "title": "Snippet Title",
      "code": "print('Hello, World!')",
      "language": "Python"
  }
  ```

#### 2. Read a Snippet
- **Method**: `GET`
- **URL**: `/api/snippets/{id}`
- **Response**:
  - **200 OK**
  ```json
  {
      "id": 1,
      "title": "Snippet Title",
      "code": "print('Hello, World!')",
      "language": "Python"
  }
  ```

#### 3. Update a Snippet
- **Method**: `PUT`
- **URL**: `/api/snippets/{id}`
- **Request Body**:
  ```json
  {
      "title": "Updated Snippet Title",
      "code": "print('Hello, Updated World!')",
      "language": "Python"
  }
  ```
- **Response**:
  - **200 OK**
  ```json
  {
      "id": 1,
      "title": "Updated Snippet Title",
      "code": "print('Hello, Updated World!')",
      "language": "Python"
  }
  ```

#### 4. Partially Update a Snippet
- **Method**: `PATCH`
- **URL**: `/api/snippets/{id}`
- **Request Body**:
  ```json
  {
      "title": "Partially Updated Snippet Title"
  }
  ```
- **Response**:
  - **200 OK**
  ```json
  {
      "id": 1,
      "title": "Partially Updated Snippet Title",
      "code": "print('Hello, Updated World!')",
      "language": "Python"
  }
  ```

#### 5. Delete a Snippet
- **Method**: `DELETE`
- **URL**: `/api/snippets/{id}`
- **Response**:
  - **204 No Content**

### Warning
- The server may take a few minutes to start up, please be patient after initiating the server.

---

## Bilingual Documentation

### Tetun
**Pundamétu**: Keta hetan_saida API Snippets, no halo ita konta ba CRUD operasaun sira.

**PUNTIANE karak:** Oin ruma **GET** talit, **POST** talit, **PUT** talit, **PATCH** talit no **DELETE** talit. Todos iha autenticasaun (token JWT).

**Fila ba Snippet**: ... *Continue with Tetun translations for each section above*