# Key Notes: Security Fundamentals

## 1. Safeguard Information

Protecting information is a core responsibility in cybersecurity. Organizations use security controls to reduce risks and ensure data remains confidential, accurate, and available.

### Key Concepts
- **Security controls:** Safeguards that reduce risks to data and systems
- **Confidentiality:** Ensuring only authorized users can access information
- **Integrity:** Ensuring data is not altered or tampered with
- **Availability:** Ensuring systems and data are accessible when needed (CIA triad)

### Common Safeguards
- Access controls (restricting who can view or use data)
- Encryption (protecting data from unauthorized reading)
- Authentication systems (verifying user identity)
- Backups and recovery systems
- Monitoring and logging for suspicious activity

### Key Idea
Information must be protected at all stages:
- At rest (stored data)
- In transit (moving across networks)
- In use (being processed)

---

## 2. Encryption Methods

Encryption is the process of converting readable data (plaintext) into an unreadable format (ciphertext) to protect it from unauthorized access.

### Key Concepts
- **Cipher:** Algorithm used to encrypt and decrypt data
- **Key:** Secret value used in encryption/decryption
- **Cryptography:** Science of securing information through encoding techniques

### Types of Encryption

#### Symmetric Encryption
- Uses a single shared key
- Same key used for encryption and decryption
- Faster and efficient for large data
- Example: AES (Advanced Encryption Standard)

**Pros:**
- High speed
- Low computational cost

**Cons:**
- Key sharing must be secure
- If key is stolen, data is compromised

---

#### Asymmetric Encryption
- Uses two keys:
  - Public key (encrypts data)
  - Private key (decrypts data)
- Used in secure communication over networks

**Examples:**
- RSA
- Digital certificates (PKI systems)

**Pros:**
- More secure key exchange
- No need to share private key

**Cons:**
- Slower than symmetric encryption

---

### Supporting Concepts
- **Hashing:** One-way transformation used for integrity checks
- **Salting:** Adds random data before hashing to increase security
- **Brute force attacks:** Attempts to guess encryption keys through trial and error

---

## 3. Authentication, Authorization, and Accounting (AAA)

AAA is a framework used to control access to systems and track user activity.

---

### 1. Authentication (Who are you?)
Verifies the identity of a user.

#### Methods:
- Something you know (password, PIN)
- Something you have (phone, token, OTP)
- Something you are (biometrics)

#### Technologies:
- MFA (Multi-Factor Authentication)
- SSO (Single Sign-On)

---

### 2. Authorization (What can you do?)
Determines what resources a user is allowed to access after authentication.

#### Access Control Models:
- **MAC (Mandatory Access Control):** Strict, system-controlled access
- **DAC (Discretionary Access Control):** Data owner decides access
- **RBAC (Role-Based Access Control):** Access based on job role

#### Principle of Least Privilege:
- Users receive only the minimum access needed to perform their job

---

### 3. Accounting (What did you do?)
Tracks user actions within a system.

#### Includes:
- Logging user activity
- Monitoring system access
- Auditing changes and behavior

---

### Key Idea
AAA ensures:
- Only the right users gain access
- They can only do what they are permitted to do
- All actions are tracked for security and compliance

---