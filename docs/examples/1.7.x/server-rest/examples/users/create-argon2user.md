POST /v1/users/argon2 HTTP/1.1
Host: cloud.appwrite.io
Content-Type: application/json
X-Appwrite-Response-Format: 1.7.0
X-Appwrite-Project: <YOUR_PROJECT_ID>
X-Appwrite-Key: <YOUR_API_KEY>

{
  "userId": "<USER_ID>",
  "email": "email@example.com",
  "password": "password",
  "name": "<NAME>"
}
