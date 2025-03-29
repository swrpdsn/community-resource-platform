# Sample Test Scenarios

These are example flows a candidate should manually test to ensure the app is working properly.

---

## ✅ Scenario 1: Full Registration + Resource Posting

1. Register a new user with email and password
2. Login using those credentials
3. Post a new resource (either a “need” or an “offer”)
4. Check if the resource appears in the listing

---

## ✅ Scenario 2: Search and Match

1. Use the search function to filter resources by category/tag
2. Check if relevant results are returned
3. Try a non-matching tag — should return empty or 404

---

## ✅ Scenario 3: Messaging Flow (if implemented)

1. Login as User A and send a message to User B
2. Login as User B and verify message is received
3. Try sending a blank message — should show an error

---

## ✅ Scenario 4: Invalid Resource Submission

1. Attempt to create a resource with missing fields
2. Verify backend returns 400 Bad Request

---

## ✅ Scenario 5: Admin View (if applicable)

1. Login as admin
2. View all resources and basic user analytics
3. Verify dashboard loads without error


