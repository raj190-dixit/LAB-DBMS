# question 1:- list all employees and jobs in Department 30 in descending order by salary
# query:- SELECT ENAME, JOB, SAL FROM EMPLOYEE WHERE DEPTNO = 30 ORDER BY SAL DESC;
![alt text](<Screenshot 2026-02-02 163128.png>)

# question 2:-List job and department number of employees whose name is five letters long, begins with 'A' and ends with 'N'
# query:-SELECT JOB, DEPTNO FROM EMPLOYEE WHERE ENAME LIKE 'A___N';
![alt text](<Screenshot 2026-02-02 163819.png>)

# question 3:-Display names of employees whose name starts with 'S'
# query :-SELECT ENAME FROM EMPLOYEE WHERE ENAME LIKE 'S%';
![alt text](<Screenshot 2026-02-02 164014.png>)

# question 4:-Display names of employees whose name ends with 'S'
# query :-SELECT ENAME FROM EMPLOYEE WHERE ENAME LIKE '%S';
![alt text](<Screenshot 2026-02-02 164052.png>)

# question 5:-Display names of employees working in department 10, 20, or 40 OR working as clerk, salesman or analyst
# query :-SELECT ENAME FROM EMPLOYEEWHERE DEPTNO IN (10, 20, 40) OR JOB IN ('CLERK', 'SALESMAN', 'ANALYST');
![alt text](image.png)

# question 6:-Display employee number and names for employees who earn commission
# query :-SELECT EMPNO, ENAME FROM EMPLOYEE WHERE COMM IS NOT NULL AND COMM > 0;
![alt text](image-1.png)

# question 7:-Display employee number and total salary for each employee
# query :-SELECT EMPNO, (SAL + NVL(COMM,0)) AS TOTAL_SALARY FROM EMPLOYEE;
![alt text](image-2.png)

# question 8:- Display employee number and annual salary for each employee
# query :-SELECT EMPNO, (SAL * 12) AS ANNUAL_SALARY FROM EMPLOYEE;
![alt text](image-3.png)

# question 9:- Display names of employees working as clerks and earning more than 3000
# query :-SELECT ENAME FROM EMPLOYEE WHERE JOB = 'CLERK' AND SAL > 3000;
![alt text](image-4.png)

# question 10:- Display names of employees who are clerk, salesman or analyst and earning more than 3000
# query :-SELECT ENAME FROM EMPLOYEE WHERE JOB IN ('CLERK', 'SALESMAN', 'ANALYST') AND SAL > 3000;
![alt text](image-5.png)