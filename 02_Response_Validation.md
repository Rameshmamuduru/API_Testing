## Response Validation

**Considerable parameters for validation**

1. Status Code
2. Headers
3. cookies
4. response time
5. response body

**To check above parameters and to validae the response we will use **Assertions****

- Assetion will use from java library called (pm)
- pm have functions, and we can call and use them by creating our own funciton (User defined Functions)
- And we will use the **Chai framework** here

**Types of User defined functions we have [Chai Framework]**
1. Normal function

```JAVA
pm.test("Test Name", functions()
            {

            }
);
```

3. Arrow function
```JAVA
pm.test("Test Name", () =>
            {

            }
);
```

## API Validation Points

**1. Validating Status Code**

- Verify whether the API returned the expected HTTP status.
- Check for a specific status code:

```
pm.test("Status code is 200", () => { 
  pm.response.to.have.status(200); 
});
```
**2. Validating Headers**
- don't need to validate every header—only headers relevant to the API specification/application requirements..
- if we have **X-Request-ID** in status code means we have header.
  
```
Content-Type
Authorization-related headers
Cache-Control
Correlation/Request ID
Security headers
```

**3. Validating Cookies**
- Not every API uses cookies. Many modern APIs use tokens such as JWT instead.
```
Cookie exists
Cookie value
Cookie expiration
Secure flag
HttpOnly
SameSite
```

- Attributes we have for the coocke security

| Attribute         | Purpose                                            |
| ----------------- | -------------------------------------------------- |
| `Secure`          | Cookie should be sent over HTTPS                   |
| `HttpOnly`        | Helps prevent JavaScript from accessing the cookie |
| `SameSite`        | Controls cross-site cookie behavior                |
| `Expires/Max-Age` | Controls cookie lifetime                           |
| `Domain`          | Controls which domain receives it                  |
| `Path`            | Controls which paths receive it                    |

**The exact attributes you validate depend on the application's security requirements.**



**4. Validating Response Time**

- Check whether the API responds within the agreed performance requirement.

**5. Validating Response Body**
- You validate the actual data returned by the API.
  - Field exists
  - Field value
  - Field isn't empty
  - Data type

**6. Validating JSON Schema**
- Schema validation checks the structure and data types of the entire response.























