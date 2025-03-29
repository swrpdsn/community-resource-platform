# API Documentation

This section includes the core API endpoints expected from your backend.

---

## 🔐 Authentication

### POST `/api/register`
- Registers a new user
- Body: `{ "name": "", "email": "", "password": "" }`

### POST `/api/login`
- Logs in a user
- Body: `{ "email": "", "password": "" }`

---

## 📦 Resources

### GET `/api/resources`
- Returns all available resources

### POST `/api/resources`
- Adds a new resource
- Body: `{ "title": "", "type": "need/offer", "description": "", "tags": [] }`

### PUT `/api/resources/:id`
- Updates a resource

### DELETE `/api/resources/:id`
- Deletes a resource

---

## 💬 Messaging (Optional)

### GET `/api/messages/:userId`
- Fetch messages with a specific user

### POST `/api/messages`
- Send a message
- Body: `{ "to": "", "message": "" }`
