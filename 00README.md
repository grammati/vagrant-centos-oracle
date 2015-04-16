TODO

```
[vagrant@localhost ~]$ cat oradiag_vagrant/diag/clients/user_vagrant/host_61728193_80/trace/sqlnet.log
Thu Apr 16 20:59:58 2015
Create Relation ADR_CONTROL
Create Relation ADR_INVALIDATION
Create Relation INC_METER_IMPT_DEF
Create Relation INC_METER_PK_IMPTS
Directory does not exist for read/write [/u01/app/oracle/product/11.2.0/xe/log] [/u01/app/oracle/product/11.2.0/xe/log/diag/clients]
```

---
TODO
Grab the 11g zip'ed RPM from 
[the Oracle site](http://www.oracle.com/technetwork/products/express-edition/downloads/index.html)
after accepting the license terms.  Copy it into the oracle directory.


---

sqlplus system/manager@vagrant

SQL> create user scott identified by tiger;

User created.

SQL> grant all privileges to scott;

Grant succeeded.

sqitch rebase  db:oracle://scott:tiger@/vagrant
