# Lab 3: SQL injection UNION attack, determining the number of columns returned by the query

- **Objective:** Find out how many columns are being returned by the original query using a `UNION` attack.
- **Payload:** 
  - `' UNION SELECT NULL--`
  - `' UNION SELECT NULL,NULL--`
  - `' UNION SELECT NULL,NULL,NULL--` (and so on)

### How I solved it:
1. Opened the target website and clicked on a product category filter to trigger the database query.
2. Intercepted the request using Burp Suite and sent it over to Repeater.
3. Tested the number of columns using two different methods:
   - **Method 1 (ORDER BY):** Injected `ORDER BY 1`, `ORDER BY 2`, `ORDER BY 3` until the application threw a database error (e.g., error at `ORDER BY 4` means there are 3 columns).
   - **Method 2 (UNION SELECT):** Injected an increasing number of `NULL` values with `UNION SELECT` until the internal server error (500) stopped and the page loaded cleanly.
4. Confirmed that appending 3 `NULL` values (`' UNION SELECT NULL,NULL,NULL--`) successfully rendered the page without errors, proving that the original query returns 3 columns.

---
![Lab 3 Proof](images/sql-lab-03.png)

