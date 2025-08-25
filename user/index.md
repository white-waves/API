# User
This section presents all requests related to user account operations.
## Register
Allows you to register a new account.
### Endpoint
```
/api/register
```
### Request
```json
{
    "login": "email@example.com",
    "password": "Pa$$w0rd!",
    "nickname": "nickname"
}
```
### Answer
```json
{
    "id": 1234567890123,
    "login": "email@example.com",
    "nickname": "nickname"
}
```
## Login
Allows you to log in to your account and create a session.
### Endpoint
```
/api/login
```
### Request
```json
{
    "login": "email@example.com",
    "password": "Pa$$w0rd!",
}
```
### Answer
```json
{
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6MTc1NjE0NDIyNzQwNywibG9naW4iOiJkb3JvbGVpam5AZ21haWwuY29tIiwibmlja25hbWUiOiJsaXVicXVhbnRpIiwiaWF0IjoxNzU2MTQ0MzYxLCJleHAiOjE3NTY3NDkxNjF9.jFrEiEkYNPNfknLZYTqSiwpBX5UhZOevmChLXiT_-8Y",
    "user": {
        "id": 1234567890123,
        "login": "email@example.com",
        "nickname": "nickname"
    }
}
```