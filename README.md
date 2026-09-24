# API_Testing

## Topics to cover for API Testing:
```
API TESTING
│
├── 1. Functional / Business Logic
├── 2. Request Validation
├── 3. Positive Scenarios
├── 4. Negative Scenarios
├── 5. Authentication
├── 6. Authorization / Access Control
├── 7. Request Headers
├── 8. Request Parameters
├── 9. Request Body / Payload
├── 10. Response Status Code
├── 11. Response Headers
├── 12. Response Body / Schema
├── 13. Error Handling
├── 14. Boundary / Limit Testing
├── 15. Data Validation
├── 16. Database / Data Integrity
├── 17. API-to-API Integration
├── 18. Security
├── 19. Session / Token Management
├── 20. Idempotency / Duplicate Requests
├── 21. Concurrency
├── 22. Performance
├── 23. Reliability / Resilience
├── 24. Compatibility
└── 25. Logging / Monitoring / Audit
```

**Where expected response codes/messages come from**

| Source                             | What you get from it                                                                          |
| ---------------------------------- | --------------------------------------------------------------------------------------------- |
| **Swagger / OpenAPI**              | Endpoints, request schema, response schema, documented status codes                           |
| **API contract**                   | Expected success/error responses and structures                                               |
| **Business requirements**          | Business rules and expected behavior                                                          |
| **Acceptance criteria**            | Specific expected outcomes                                                                    |
| **Jira stories**                   | Requirements and sometimes error scenarios                                                    |
| **Developer/API team**             | Missing/unclear response codes and behavior                                                   |
| **Existing Postman collection**    | Existing requests, examples, environments                                                     |
| **Actual API execution**           | Actual response; useful for discovering behavior, but not automatically the expected behavior |
| **Database/service documentation** | Data/state behavior and integration expectations                                              |




















