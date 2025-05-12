# sit323-2024-prac9p
# Cloud Native Application with MongoDB Integration

## Overview
This project integrates MongoDB with a Node.js application deployed in Kubernetes. The application performs basic CRUD operations on MongoDB.

## Prerequisites
- Kubernetes cluster
- Docker
- kubectl
- MongoDB client libraries (e.g., Mongoose for Node.js)

## Setup
1. Clone the repository.
2. Build Docker images using the provided Dockerfile.
3. Deploy the MongoDB container in Kubernetes.
4. Deploy the application container in Kubernetes.
5. Create Persistent Volumes and Secrets for MongoDB.
6. Test CRUD operations.

## Kubernetes Deployment Instructions
- Apply the MongoDB and application deployment manifests using `kubectl apply -f`.
- Access the application through the exposed service.

## Testing
Use Postman or Curl to test the CRUD operations:
- Create an item: `POST /items`
- Get items: `GET /items`
- Update an item: `PUT /items/:id`
- Delete an item: `DELETE /items/:id`

## Backup and Recovery
MongoDB backups are handled using `mongodump` and stored in a persistent volume. Recovery instructions are documented here.
