# question 1:- Display total number of employees
# query :-SELECT COUNT(*) AS TOTAL_EMPLOYEES FROM EMPLOYEE;
![alt text](image.png)

# question 2:- Display total salary paid to all employees
# query :-SELECT SUM(SAL) AS TOTAL_SALARY FROM EMPLOYEE;
![alt text](image-1.png)

# question 3:- Display maximum salary
# query :-SELECT MAX(SAL) AS MAX_SALARY FROM EMPLOYEE;
![alt text](image-2.png)

# question 4:-Display minimum salary
# query :-SELECT MIN(SAL) AS MIN_SALARY FROM EMPLOYEE;
![alt text](image-3.png)

# question 5:-Display average salary
# query :-SELECT AVG(SAL) AS AVG_SALARY FROM EMPLOYEE;
![alt text](image-4.png)

# question 6:-Display maximum salary of clerks
# query :-SELECT MAX(SAL) FROM EMPLOYEE WHERE JOB = 'CLERK';
![alt text](image-5.png)

# question 7:-Display maximum salary in department 20
# query :-SELECT MAX(SAL) FROM EMPLOYEE WHERE DEPTNO = 20;
![alt text](image-6.png)

# question 8 :-Display minimum salary of salesman
# query :-SELECT MIN(SAL) FROM EMPLOYEE WHERE JOB = 'SALESMAN';
![alt text](image-7.png)

# question 9:-Display average salary of managers
# query :-SELECT AVG(SAL) FROM EMPLOYEE WHERE JOB = 'MANAGER';
![alt text](image-8.png)

# question 10:-Display total salary of analysts in department 40
# query :-SELECT SUM(SAL) FROM EMPLOYEE WHERE JOB = 'ANALYST' AND DEPTNO = 40;
![alt text](image-9.png)

# question 11:-Display employee names in uppercase
# query :-SELECT UPPER(ENAME) FROM EMPLOYEE;
![alt text](image-10.png)

# question 12:-Display employee names in lowercase
# query :-SELECT LOWER(ENAME) FROM EMPLOYEE;
![alt text](image-11.png)

# question 13:-Display employee names in proper case
# query :-SELECT INITCAP(ENAME) FROM EMPLOYEE;


# question 14:-Display length of your name
# query :-SELECT LENGTH('RAJ') AS NAME_LENGTH FROM DUAL;
![alt text](image-12.png)

# question 15:-Display length of all employee names
# query :-SELECT ENAME, LENGTH(ENAME) FROM EMPLOYEE;
![alt text](image-13.png)
