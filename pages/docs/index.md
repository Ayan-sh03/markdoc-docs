# Registration API

This API Uses [JWT](https://jwt.io) (Json Web Token ) for Authentication and OTP based Email Verifications

---

# Register

User can Register an Account using Their Email Address , Secure Password, First Name, Last Name and Middle Name (optional )

## Request

```json
{
  "email": "john@example.com",
  "first_name": "John",
  "last_name": "doe",
  "middle_name": "jane",
  "password": "secureP@ss!124"
}
```

## Response

```json
{
  "email": "john@example.com",
  "first_name": "John",
  "last_name": "doe",
  "middle_name": "jane"
}
```

## Erros
