# mysql

show variables  :-- To see all the variable option which can configurable 

Ex: - show variables like 'innodb_lock_wait_timeout';


Unlocking tables in mysql

1) Enter MySQL

mysql -u your_user -p
2) Let's see the list of locked tables

mysql> show open tables where in_use>0;
3) Let's see the list of the current processes, one of them is locking your table(s)

mysql> show processlist;
4) Let's kill one of these processes

mysql> kill put_process_id_here;



