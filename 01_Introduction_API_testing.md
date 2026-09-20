## API Testing:

API Testing means testing the backend APIs directly to verify that they correctly process requests, apply business rules, and return the expected responses.

**In simple terms:**

UI testing checks what the user sees. API testing checks what happens behind the UI.

## Client-Server Architecture

Client-server architecture is a system design where one system (the client) requests a service/data from another system (the server), and the server processes the request and 
sends back a response.

```
CLIENT
   |
   | Request
   ↓
SERVER
   |
   | Response
   ↓
CLIENT
```
**Who is Client**
A client is system/application that initiate the request for service/data.

**Example**
``` TEXT
Web Browser
Mobile App
Desktop Application
Postman
Another Backend Application
IoT Device
```

**Who is a Server**

A server is a system/application that receives requests, processes them, and provides a response or service.

**Example**
```
Client
  ↓
"Give me account balance"
  ↓
Server
  ↓
"Your balance is ₹50,000"
```

**Business Flow**
```
Browser
   ↓
Frontend
   ↓
API
   ↓
Backend
   ↓
Database
```
**Browser**

Client.

**Frontend**

Part of the client-side application.

**API**

The communication interface through which the client communicates with the server-side application.

**Backend application**

Server-side application.

**Database**

Stores data used by the server.

**Simple API request and response Flow**

```
CLIENT
   |
   | Request
   |
   | Method: GET
   | URL: /api/accounts/123
   | Headers
   | Authentication
   ↓
SERVER
   |
   | Process
   | Validate
   | Business Logic
   | Database
   |
   ↓
CLIENT
   |
   | Response
   |
   | Status: 200
   | Headers
   | JSON Body
   ↓
```

**Client-server architecture is a communication model where a client sends a request to a server, the server processes that request—often using business logic, databases, or other services—and sends a response back to the client.**
















































