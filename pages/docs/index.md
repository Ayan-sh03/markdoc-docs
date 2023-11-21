# Registration API

This API Uses [JWT](https://jwt.io) (Json Web Token ) for Authentication and OTP based Email Verifications

---

# Register

User can Register an Account using Their Email Address , Secure Password, First Name, Last Name and Middle Name (optional )

## Request

Body :

```js
{
  "email": "john@example.com",
  "first_name": "John",
  "last_name": "doe",
  "middle_name": "jane",
  "password": "secureP@ss!124"
}
```

## Response

Body :

```javascript
{
  "email": "john@example.com",
  "first_name": "John",
  "last_name": "doe",
  "middle_name": "jane"
}
```

## Errors

Error Body :

```js
{
  "error":"Error Message"
}
```

{% table %}

- HTTP Error Summary

---

- 400
- Bad Request - Invalid JSON Data , Invalid Email

---

- 409
- Conflict - User Already Exists

---

- 500
- Internal Server Error - Something went wrong with the server

---

{% /table %}
