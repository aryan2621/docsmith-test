---
title: "API Reference"
order: 2
---

# API Reference

Complete API documentation for the platform.

## Authentication

All API requests require a bearer token:

```http
Authorization: Bearer <token>
```

## Endpoints

### GET /api/projects

List all projects for the authenticated user.

**Response:**
```json
[
  {
    "id": 1,
    "name": "My Project",
    "slug": "my-project"
  }
]
```

### POST /api/projects

Create a new project.

**Body:**
```json
{
  "name": "New Project",
  "slug": "new-project"
}
```

## Error Handling

Errors follow a consistent format:

```json
{
  "error": "Error message",
  "code": "ERROR_CODE"
}
```
