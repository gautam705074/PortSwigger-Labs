# 🔬 02 - Stored XSS into HTML context with nothing encoded

## 📌 Lab Details
- **Description:** This lab contains a stored cross-site scripting vulnerability in the comment functionality.
- **Reference:** https://portswigger.net/web-security/cross-site-scripting/stored
- **Payload Used:** `<script>alert(1)</script>`

## 🛠️ Step-by-Step Solution
1. Visited a blog post and found a comment section that takes user input (Name, Email, Comment, Website).
2. Injected the payload `<script>alert(1)</script>` into the comment field.
3. Submitted the comment and navigated back to the blog post page.
4. Verified that the stored script executed and the alert box popped up when the comment was rendered.

---

## 🖼️ Lab Proof / Screenshot
![XSS Lab 2 Proof](images/xss-lab-02.png)
