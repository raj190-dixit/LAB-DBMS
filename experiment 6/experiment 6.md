# question 1:-Display empno, ename, deptno from employee table. Instead of display department numbers display the related department name (Use decode function).
# query - SELECT EMPNO, ENAME, CASE WHEN DEPTNO = 10 THEN 'RESEARCH' WHEN DEPTNO = 20 THEN 'ACCOUNTING' WHEN DEPTNO = 30 THEN 'SALES' WHEN DEPTNO = 40 THEN 'OPERATIONS' ELSE 'UNKNOWN' END AS DNAME FROM EMPLOYEE;
![alt text](image.png)

# question 2:-Display your age in days.
# query - SELECT DATEDIFF(CURDATE(), '2000-01-01') AS AGE_DAYS;
![alt text](image-1.png)

# question 3:-Display your age in months. 1,2
# query - SELECT TIMESTAMPDIFF(MONTH, '2000-01-01', CURDATE()) AS AGE_MONTHS;
![alt text](image-2.png)

# question 4:-Display the current date as 15th August Friday Nineteen Ninety-Seven.
# query - SELECT DATE_FORMAT(CURDATE(), '%D %M %W %Y') AS FORMATTED_DATE;
![alt text](image-3.png)

# question 5:-Display the following output for each row from employee table.
# query - SELECT CONCAT(ENAME, ' has joined the company on ', DATE_FORMAT(HIREDATE, '%W %D %M %Y')) AS INFO FROM EMPLOYEE;
![alt text](image-4.png)

# question 6:-Scott has joined the company on Wednesday 13th August Nineteen Ninety
# query - SELECT CONCAT('Scott has joined the company on ', DATE_FORMAT(HIREDATE, '%W %D %M %Y')) FROM EMPLOYEE WHERE ENAME = 'SCOTT';
![alt text](image-5.png)

# question 7:-Find the date for nearest Saturday after current date.
# query -SELECT DATE_ADD(CURDATE(), INTERVAL (7 - DAYOFWEEK(CURDATE())) % 7 DAY) AS NEXT_SATURDAY;
![alt text](image-6.png)


# question 8:-Display current time.
# query -SELECT CURTIME() AS TIME_NOW;
![alt text](image-7.png)

# question 9:-Display the date three months Before the current date
# query -SELECT DATE_SUB(CURDATE(), INTERVAL 3 MONTH) AS THREE_MONTHS_BEFORE;
![alt text](image-8.png)

# question 10:-Display those employees who joined in the company in the month of Dec.
# query - SELECT * FROM EMPLOYEE WHERE MONTH(HIREDATE) = 12;
![alt text](image-9.png)

# question 11:-Display those employees whose first 2 characters from hire date -last 2 characters of salary.
# query -SELECT ENAME, CONCAT(LEFT(DATE_FORMAT(HIREDATE,'%d%m%y'),2), RIGHT(SAL,2)) AS RESULT FROM EMPLOYEE;
![alt text](image-10.png)

# question 12:-Display those employees whose 10% of salary is equal to the year of joining.
# query -SELECT * FROM EMPLOYEE WHERE (SAL * 0.10) = RIGHT(YEAR(HIREDATE),2);
![alt text](image-11.png)

# question 13:-Display those employees who joined the company before 15 of the months.
# query -SELECT * FROM EMPLOYEE WHERE DAY(HIREDATE) < 15;
![alt text](image-12.png)

# question 14:-Display those employees who has joined before 15th of the month
# query -SELECT * FROM EMPLOYEE WHERE DAY(HIREDATE) < 15;
![alt text](image-13.png)

# question 15:-Display those employees whose joining DATE is available in deptno
# query - SELECT * FROM EMPLOYEE WHERE DAY(HIREDATE) = DEPTNO;
![alt text](image-14.png)