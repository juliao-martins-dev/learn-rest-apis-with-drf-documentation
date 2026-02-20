# API Documentation

This document provides comprehensive details about the REST API available at the endpoint [https://juliao-martins-snippets.onrender.com/](https://juliao-martins-snippets.onrender.com/).

## Table of Contents
- [General Information](#general-information)
- [API Endpoints](#api-endpoints)
  - [GET Method](#get-method)
  - [POST Method](#post-method)
  - [PUT Method](#put-method)
  - [PATCH Method](#patch-method)
  - [DELETE Method](#delete-method)
- [Server Startup Time](#server-startup-time)

## General Information
This API is designed to manage resources effectively, supporting various HTTP methods to interact with them. Please ensure to check the respective headers and payload requirements for each method.

## API Endpoints

### GET Method
- **Endpoint:** `/resource`
- **Description:** Retrieves a list of resources.
- **Response:** 200 OK (returns JSON array of resources)

### POST Method
- **Endpoint:** `/resource`
- **Description:** Creates a new resource.
- **Request Body:** JSON object containing the details of the resource to create.
- **Response:** 201 Created (returns the created resource)
  
### PUT Method
- **Endpoint:** `/resource/{id}`
- **Description:** Updates an existing resource by replacement.
- **Request Body:** JSON object containing the updated details of the resource.
- **Response:** 200 OK (returns the updated resource)

### PATCH Method
- **Endpoint:** `/resource/{id}`
- **Description:** Updates partial details of an existing resource.
- **Request Body:** JSON object containing the fields to update.
- **Response:** 200 OK (returns the updated resource)

### DELETE Method
- **Endpoint:** `/resource/{id}`
- **Description:** Deletes a resource.
- **Response:** 204 No Content (successful deletion)

## Server Startup Time
Be aware that the server may take some time to start up. Depending on the environment and current load, it may take some seconds to respond to the first request once it is started. Please plan your interactions accordingly to accommodate for this delay.