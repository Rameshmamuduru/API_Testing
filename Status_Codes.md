## 200 Series Status Codes

| Status Code                           | Meaning                                                                                                  | When it is used                                                              | Example                                                                       |
| ------------------------------------- | -------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| **200 OK**                            | Request was successful                                                                                   | GET, PUT, PATCH, or sometimes POST when the operation completes successfully | `GET /users/101` → User details returned                                      |
| **201 Created**                       | A new resource was successfully created                                                                  | Usually after a POST request                                                 | `POST /users` → New user created with ID `102`                                |
| **202 Accepted**                      | Request was accepted for processing, but processing is not completed yet                                 | Asynchronous/background operations                                           | `POST /payments` → Payment request accepted; processing happens in background |
| **203 Non-Authoritative Information** | Request succeeded, but the returned information may have been modified or transformed by an intermediary | Proxy/cache transformation scenarios                                         | Client requests data → proxy returns modified metadata/content                |
| **204 No Content**                    | Request was successful, but there is no response body                                                    | Common with DELETE or updates where nothing needs to be returned             | `DELETE /users/102` → User deleted, response has no body                      |
| **205 Reset Content**                 | Request succeeded and the client should reset the current view/form                                      | Form submission scenarios                                                    | `POST /form` → Successfully submitted; UI should clear/reset the form         |
| **206 Partial Content**               | Server returns only part of the requested resource                                                       | Range requests, especially large files/videos                                | Client requests bytes `0–999` → Server returns only that portion              |

**Importent for API Testing**

| Code    | Remember it as             | Typical API          |
| ------- | -------------------------- | -------------------- |
| **200** | Successful request         | GET / PUT / PATCH    |
| **201** | Resource created           | POST                 |
| **202** | Accepted, processing later | Async POST           |
| **204** | Success, no response body  | DELETE / PUT / PATCH |

