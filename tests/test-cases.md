# Test Cases

Below are sample test cases to validate the core features of your application.

---

## ✅ User Registration

**Test Case 1:** Register with valid details  
- **Input:** `{ "name": "John", "email": "john@example.com", "password": "12345678" }`  
- **Expected:** 201 Created, JWT token returned

**Test Case 2:** Register with existing email  
- **Input:** `{ "name": "John", "email": "john@example.com", "password": "newpass123" }`  
- **Expected:** 409 Conflict, error message

---

## ✅ Login

**Test Case 3:** Login with correct credentials  
- **Expected:** 200 OK, JWT returned

**Test Case 4:** Login with wrong password  
- **Expected:** 401 Unauthorized

---

## ✅ Resource Creation

**Test Case 5:** Add valid resource  
- **Input:** `{ "title": "Oxygen Cylinder", "type": "offer", "description": "Available in Mumbai", "tags": ["medical"] }`  
- **Expected:** 201 Created

**Test Case 6:** Missing fields  
- **Input:** `{ "title": "Oxygen Cylinder" }`  
- **Expected:** 400 Bad Request

---

## ✅ Matching Algorithm

**Test Case 7:** Match based on category/tag  
- **Input:** Search with tag `medical`  
- **Expected:** Returns matching resources

---

## ✅ Messaging (Optional)

**Test Case 8:** Send message  
- **Input:** `{ "to": "userId123", "message": "Hi, I can help you." }`  
- **Expected:** 200 OK, message saved
