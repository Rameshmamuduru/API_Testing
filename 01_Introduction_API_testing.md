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



## Types of API's:

1. **REST** → very important (Support all types) - Latest
2. **SOAP** → important, especially BFSI/enterprise (Support only xml Data) - Very Old
3. **GraphQL** → good to know
4. **WebSocket** → learn when real-time applications require it
5. **gRPC** → learn after you understand REST and microservices


### REST Api:

A REST API is an API designed according to REST (Representational State Transfer) principles that allows clients and servers to communicate over HTTP using resources, URLs, and standard HTTP methods such as GET, POST, PUT, PATCH, and DELETE.

```
REST API
│
├── Resources
│    └── /customers/101
│
├── HTTP Methods
│    ├── GET
│    ├── POST
│    ├── PUT
│    ├── PATCH
│    └── DELETE
│
├── HTTP Status Codes
│    ├── 200
│    ├── 201
│    ├── 400
│    ├── 401
│    ├── 404
│    └── 500
│
├── Headers
├── Request Body
├── Response Body
└── Stateless communication
```

**API vs Web Service**

All Web services are API but All API's Are not web service.

| API                                          | Web Service                                                  |
| -------------------------------------------- | ------------------------------------------------------------ |
| Broad concept                                | Specific type of API                                         |
| Allows software-to-software communication    | Allows software-to-software communication over a network/web |
| Doesn't necessarily require internet/network | Network communication is fundamental                         |
| Can be local                                 | Remote/network-based                                         |
| Example: Java API                            | Example: SOAP Web Service                                    |
| Example: OS API                              | Example: REST Web API                                        |

**An API is an interface that enables communication between different software components, whereas a Web Service is a type of API that is exposed over a network and allows applications to communicate using web-based protocols.**












































