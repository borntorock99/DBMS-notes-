# DBMS-notes-
this is the class notes of database management system

-----------------------------------------------

Different state of transactions ( 1. active , 2. commit , 3. partially commit 4. failed )
Their could be 3 cases to perform this operations 
	1. Active --> partially commit --> failed --> abort
	2. Active --> partially commit --> commit 
	3. Active --> failed  --> abort

Concurrent transaction --- it start from same path i
Schedule -- collection of transaction 
	1. Serial schedule --  
	2. Concurrent Schedule -- 


Cascading rollbacks --- a single transactions failure lead to the rollbacks 

Recoverable schedule -- if daared epended racataons 
Cascading rollbacks --
------------------------------------------------
concurrecy control block 

1. Lock based protocols 
2. Timestamp based protocols
3. Validation based protocols 
	1. Multiple granualy 
4. Multiversion schemes 
5. Insert and delete oeprations
6. Concurrency in index strucutures 


read (shared lock)
write (exclusive lock)


lock based protocols --

a transacitons may be granted 


exampes of tracsations performing looking 
* lock s(a);
* read (a);
* unlock(b);
* lock -s(A)
* read (b);
* unlock (b);
* display(a+b);
these above points are combatabiloity blocks 




pitfalls lock based protocols 

neither t2 nor t4 can make progress executing lock -s (b) couses t4 to wait to t2 to relase its lock b while excutiig=ng lock -x (A)cuases t2 to wait for to realsease its lock onm a are ..






