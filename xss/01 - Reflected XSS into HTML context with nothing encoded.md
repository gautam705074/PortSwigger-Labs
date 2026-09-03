# 🔬 01 - Reflected XSS into HTML context with nothing encoded

## 📌 Lab Details
- **Description:** This lab contains a simple reflected cross-site scripting vulnerability in the search functionality.
- **Reference:** https://portswigger.net/web-security/cross-site-scripting/reflected
- **Payload Used:** `<script>alert(1)</script>`

## 🛠️ Step-by-Step Solution
1. Intercepted the search request using Burp Suite or typed directly into the search functionality.
2. Searched for the payload: `<script>alert(1)</script>`
3. Verified that the script executed and the alert box popped up.

---

## 🖼️ Lab Proof / Screenshot
![XSS Lab 1 Proof](images/xss-lab-01.png)
