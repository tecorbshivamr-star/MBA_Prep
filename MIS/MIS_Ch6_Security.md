# 📗 MIS CHAPTER 6: Information Systems Security
### Subject: Management of Information Systems | MBA 2nd Semester | DU SOL
**From Beginner → Exam Ready**

---

## 🟢 BEGINNER LEVEL — "What is this about?"

If a bank leaves its vault open, robbers will steal physical cash. 
Today, data is far more valuable than physical cash. If an airline's database is hacked, the hacker can steal the credit card numbers and passport details of a million passengers. The airline will be sued for billions of dollars and destroyed. 

**Information Security (InfoSec)** is the digital vault. It is the practice of defending computers, servers, mobile devices, networks, and data from malicious cyberattacks. 

---

## 🟡 INTERMEDIATE LEVEL — "Key Concepts & Frameworks"

### 1. The CIA Triad (The Golden Rule of Security)
Every security system must guarantee three things:
- **Confidentiality:** Only *authorized* people can read the data. (A hacker cannot read your medical records).
- **Integrity:** The data is accurate and *unaltered*. (A hacker cannot change your bank balance from ₹100 to ₹1,000,000).
- **Availability:** The system is actually *working* when you need it. (If you need to withdraw cash, the ATM system must be online, not crashed by an attack).

### 2. Types of Cyber Attacks
- **Phishing:** An email that *looks* exactly like it's from HDFC Bank, asking you to click a link and enter your password. Once you do, the hacker steals it.
- **Ransomware:** A virus that locks all the files on your computer. A message pops up saying, "Pay us $50,000 in Bitcoin, or we will delete everything."
- **DDoS (Distributed Denial of Service):** A hacker uses a million fake computers to try and log into a website at the exact same second. The website's servers get overwhelmed and crash. 
- **Insider Threat:** The most dangerous attack. An angry employee legally logs in and downloads the company's secret data onto a USB drive.

### 3. Encryption (Secret Codes)
Encryption is scrambling a message so nobody can read it except the person with the "key." 
- **Symmetric:** Like a house key. The sender and receiver use the *exact same key* to lock and unlock the file.
- **Asymmetric:** Like a mailbox. You have a **Public Key** (anyone can drop a letter in the slot) and a **Private Key** (only YOU have the key to open the box and read the letters). 

---

## 🔴 ADVANCED / EXAM LEVEL — "How to write it in the exam?"

### Q. What is the CIA Triad in Information Security? Discuss any three major cybersecurity threats faced by modern enterprises. Differentiate between Symmetric and Asymmetric Encryption. (15 Marks)

**1. The CIA Triad of Information Security:**
The CIA Triad is the foundational model for the development of security policies within an organization. All security controls are designed to protect at least one of these three core principles:
*   **Confidentiality:** Ensuring that sensitive information is strictly protected from unauthorized access or disclosure (e.g., using strong passwords, biometric access, and data encryption).
*   **Integrity:** Ensuring that data is accurate, trustworthy, and has not been maliciously or accidentally altered during storage or transit (e.g., using hashing algorithms and strict access controls).
*   **Availability:** Ensuring that the information systems and data are readily accessible to authorized users whenever they need them (e.g., maintaining redundant backup servers and disaster recovery plans to survive hardware failures or cyberattacks).

**2. Major Cybersecurity Threats:**
*   **A. Ransomware:** 
    *   *Concept:* A type of malicious software that violently encrypts an organization's critical databases and servers, rendering them totally inaccessible. The attackers demand a massive financial ransom (usually in untraceable cryptocurrency) in exchange for the decryption key.
    *   *Impact:* In 2022, AIIMS Delhi suffered a devastating ransomware attack that paralyzed patient management and wiped out digital medical records for weeks.
*   **B. Social Engineering & Phishing:**
    *   *Concept:* Bypassing technical firewalls by manipulating human psychology. Phishing involves sending fraudulent emails disguised as legitimate corporate communications to trick employees into willingly handing over their login credentials. 
    *   *Impact:* It remains the #1 root cause of corporate data breaches because human error is harder to patch than software bugs.
*   **C. DDoS (Distributed Denial of Service):**
    *   *Concept:* An attack specifically targeting the **Availability** pillar of the CIA Triad. Attackers hijack a "botnet" (thousands of infected computers) to flood a target web server with a massive tsunami of fake internet traffic, overwhelming its capacity and causing the website to crash for legitimate customers.

**3. Symmetric vs. Asymmetric Encryption:**
Encryption is the cryptographic process of converting plaintext into unreadable ciphertext using a mathematical algorithm and a key.

*   **Symmetric Encryption (Secret-Key):**
    *   Uses a **single, shared key** for both encryption and decryption. 
    *   *Advantage:* It is computationally fast and highly efficient for encrypting massive databases.
    *   *Disadvantage:* The "Key Distribution Problem." If the sender and receiver are far apart, securely transmitting the shared key over the internet without it being intercepted by a hacker is extremely difficult. (Example standard: AES-256).
*   **Asymmetric Encryption (Public-Key):**
    *   Uses a mathematically linked **pair of keys**: a Public Key and a Private Key.
    *   *Process:* Anyone can use your widely published Public Key to encrypt a message and send it to you. However, *only* your closely guarded Private Key can decrypt and read it.
    *   *Advantage:* Completely solves the key distribution problem. You never have to share your private key over the internet. It is the foundation of secure web browsing (HTTPS/SSL) and Digital Signatures.
    *   *Disadvantage:* It is mathematically intense and computationally very slow compared to symmetric encryption. (Example standard: RSA).

**Conclusion:**
In the digital age, Information Security is no longer an IT issue; it is a critical board-level business risk. A single breach of confidentiality can destroy decades of corporate reputation and result in massive regulatory fines.
