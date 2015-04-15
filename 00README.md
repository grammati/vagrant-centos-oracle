sqlplus system/manager@vagrant

SQL> create user scott identified by tiger;

User created.

SQL> grant all privileges to scott;

Grant succeeded.

sqitch rebase  db:oracle://scott:tiger@/vagrant
