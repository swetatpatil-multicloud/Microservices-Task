# Cloud and Containers

## Microservices Containerization using Docker

## Overview
This project demonstrates containerization of a microservices-based application using Node.js, Docker, and Docker Compose.

The application consists of:
- User Service (Port 3000)
- Product Service (Port 3001)
- Gateway Service (Port 3003)

---

## Technologies Used
- Node.js
- Docker
- Docker Compose

---

## Setup Instructions

Step 1: Clone Repository
git clone https://github.com/mohanDevOps-arch/Microservices-Task.git
cd Microservices-Task

Step 2: Run Application
docker-compose up --build

### Services Access
ServiceURLUser Servicehttp://localhost:3000Product Servicehttp://localhost:3001Gateway Servicehttp://localhost:3003

### Expected Output

user-service     | Server running on port 3000
product-service  | Server running on port 3001
gateway-service  | Gateway running on port 3003

### Test in Browser

Open browser > Hit the above URLs > Ensure responses are received
http://localhost:3000 → User Service
http://localhost:3001 → Product Service
http://localhost:3003 → Gateway Service

### Troubleshooting
Containers not starting > Run docker-compose down and retry
Module errors > Run npm install locally

### Screenshots showing running containers and browser output)

<img width="940" height="743" alt="image" src="https://github.com/user-attachments/assets/ac1e6d58-7666-468e-81dc-68be7bd9ca9b" />

<img width="1906" height="577" alt="image" src="https://github.com/user-attachments/assets/0acf6098-2441-46fd-a0c2-b61ce4794729" />

<img width="1909" height="617" alt="image" src="https://github.com/user-attachments/assets/e7303ff8-7f56-4d83-95e3-d9884c383cff" />

<img width="1916" height="615" alt="image" src="https://github.com/user-attachments/assets/9d4956cb-6ee2-4b09-a04e-6a4b8550a2d9" />

<img width="1919" height="577" alt="image" src="https://github.com/user-attachments/assets/dbad6500-d50b-4901-ab06-de3ab86cca6f" />

<img width="1905" height="652" alt="image" src="https://github.com/user-attachments/assets/a1c38c76-733f-476d-9ab2-63b3db141908" />

### **User Service**
- **Base URL:** `http://localhost:3000`
- **Endpoints:**
  - **List Users:**  
    ```
    curl http://localhost:3000/users
    ```
    Or open in your browser: [http://localhost:3000/users](http://localhost:3000/users)

---

### **Product Service**
- **Base URL:** `http://localhost:3001`
- **Endpoints:**
  - **List Products:**  
    ```
    curl http://localhost:3001/products
    ```
    Or open in your browser: [http://localhost:3001/products](http://localhost:3001/products)

---

### **Order Service**
- **Base URL:** `http://localhost:3002`
- **Endpoints:**
  - **List Orders:**  
    ```
    curl http://localhost:3002/orders
    ```
    Or open in your browser: [http://localhost:3002/orders](http://localhost:3002/orders)

---

### **Gateway Service**
- **Base URL:** `http://localhost:3003/api`
- **Endpoints:**
  - **Users:**  
    ```
    curl http://localhost:3003/api/users
    ```
  - **Products:**  
    ```
    curl http://localhost:3003/api/products
    ```
  - **Orders:**  
    ```
    curl http://localhost:3003/api/orders
    ```

---

## Instructions
1. Start all services using the `docker-compose` file:
   ```
   docker-compose up --build
   ```
2. Once the services are running, use the above endpoints to verify the functionality.

## Author
Sweta Patil
