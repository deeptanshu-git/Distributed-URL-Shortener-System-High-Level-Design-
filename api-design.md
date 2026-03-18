## 🔌 APIs

### 1. Create Short URL

**POST /shorten**

- Description: Generates a short URL from the original URL

**Request Body:**
- originalUrl (string)
- userId (long)
- apiKey (string)
- expiry (date)

**Response:**
- shortUrl (string)

---

### 2. Delete URL

**DELETE /url**

- Description: Deletes an existing short URL

**Request Body:**
- apiKey (string)
- originalUrl (string)
- shortUrl (string)

**Response:**
- success (boolean)

---

### 3. User Signup

**POST /signup**

- Description: Registers a new user

**Request Body:**
- name (string)
- email (string)
- password (string)

**Response:**
- userId (long)
- apiKey (string)

---

### 4. User Login

**POST /login**

- Description: Authenticates user and returns API key

**Request Body:**
- email (string)
- password (string)

**Response:**
- apiKey (string)

---

### 5. User Logout

**POST /logout**

- Description: Invalidates user session

**Request Body:**
- apiKey (string)

**Response:**
- success (boolean)
