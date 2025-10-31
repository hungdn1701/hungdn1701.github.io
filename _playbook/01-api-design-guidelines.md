---
title: "RESTful API Design Guidelines"
category: "API Design"
order: 1
description: "Best practices and standards for designing consistent, maintainable REST APIs."
tags: ["REST", "API", "HTTP", "Design"]
updated: 2024-10-15
---

## Naming Conventions

### Resources

- Use **plural nouns** for collections: `/users`, `/products`, `/orders`
- Use **kebab-case** for multi-word resources: `/product-categories`
- Avoid verbs in URLs (use HTTP methods instead)

```
✅ GET /users/123
❌ GET /getUser/123
```

### Query Parameters

- Use **snake_case** for consistency: `?sort_by=date&page_size=20`
- Support standard pagination: `page`, `page_size` or `offset`, `limit`

## HTTP Methods

| Method | Usage | Idempotent |
|--------|-------|------------|
| GET | Retrieve resources | ✅ |
| POST | Create new resource | ❌ |
| PUT | Update/replace resource | ✅ |
| PATCH | Partial update | ❌ |
| DELETE | Remove resource | ✅ |

## Response Format

### Success Response

```json
{
  "data": { ... },
  "meta": {
    "timestamp": "2024-10-15T10:30:00Z",
    "version": "1.0"
  }
}
```

### Error Response

```json
{
  "error": {
    "code": "VALIDATION_ERROR",
    "message": "Invalid email format",
    "details": [
      {
        "field": "email",
        "issue": "Must be a valid email address"
      }
    ]
  }
}
```

## Status Codes

- **200 OK**: Successful GET, PUT, PATCH
- **201 Created**: Successful POST
- **204 No Content**: Successful DELETE
- **400 Bad Request**: Client error (validation)
- **401 Unauthorized**: Authentication required
- **403 Forbidden**: Insufficient permissions
- **404 Not Found**: Resource doesn't exist
- **500 Internal Server Error**: Server error

## Versioning

Use URL versioning for major breaking changes:
```
/api/v1/users
/api/v2/users
```

## Pagination

```
GET /api/v1/products?page=2&page_size=20

Response:
{
  "data": [...],
  "pagination": {
    "page": 2,
    "page_size": 20,
    "total_items": 150,
    "total_pages": 8
  }
}
```

## Filtering and Sorting

```
GET /api/v1/products?category=electronics&sort_by=price&order=asc
```

## Best Practices

1. **Always validate input** at the API layer
2. **Use appropriate status codes** for different scenarios
3. **Document your API** with OpenAPI/Swagger
4. **Version your APIs** from the start
5. **Implement rate limiting** to prevent abuse
6. **Use HTTPS** in production
7. **Implement proper error handling** with meaningful messages
8. **Support CORS** for web clients when needed
