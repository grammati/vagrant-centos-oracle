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
