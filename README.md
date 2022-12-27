# DBMS_LABQUES
DBMS  lab question answer
WEEK 5 & 6 
Question no.3 = Write a query to display employee id, employee name, salary, department name and project completion date from the above relations.
sql command= 
//

SELECT EMP21013.EID, EMP21013.ENAME, EMP21013.SALARY, DEPT21013.DNAME, WORKS21013.PCDATE
FROM EMP21013
INNER JOIN WORKS21013 ON EMP21013.EID = WORKS21013.EID
INNER JOIN DEPT21013 ON DEPT21013.DID = WORKS21013.DID

//

Question 4 = Write a query to display the names of all manager along their department name and department id.
sql command=
// 

select EMP21013.ENAME, DEPT21013.MANAGERID, DEPT21013.DNAME, DEPT21013.DID
FROM EMP21013
INNER JOIN DEPT21013 ON EMP21013.EID = DEPT21013.MANAGERID

//

Question 6 = Display the name of employee along with their department names.
sql command=
//

SELECT EMP21013.ENAME, DEPT21013.DNAME
FROM EMP21013
INNER JOIN WORKS21013 ON EMP21013.EID = WORKS21013.EID
INNER JOIN DEPT21013 ON DEPT21013.DID = WORKS21013.DID

//
