# 🔬 03 - DOM XSS in document.write sink using source location.search

## 📌 Lab Details
- **Description:** This lab contains a DOM-based cross-site scripting vulnerability in the search tracking functionality. It uses the JavaScript `document.write` sink, which reads from the `location.search` source.
- **Reference:** https://portswigger.net/web-security/cross-site-scripting/dom
- **Payload Used:** `"><script>alert(1)</script>`

## 🛠️ Step-by-Step Solution
1. Visited the home page and used the search functionality.
2. Injected a random search term and inspected the source code to find that input is processed via `document.write` from `location.search`.
3. Injected the payload `"><script>alert(1)</script>` to break out of the existing HTML context.
4. Verified that the script executed and the alert box popped up.

---

## 🖼️ Lab Proof / Screenshot
![XSS Lab 3 Proof](images/xss-lab-03.png)
