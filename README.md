1.SELECT Name 
FROM Employees
WHERE Salary > ( SELECT 
                AVG(Salary) 
                FROM Employees)

2.SELECT Name 
FROM Employees
WHERE Salary = ( SELECT 
                MAX(Salary) 
                FROM Employees)

3.SELECT Name 
FROM Employees
WHERE Salary < ( SELECT 
                AVG(Salary) 
                FROM Employees)


4.SELECT Name , Department
FROM Employees
WHERE Department IN ( SELECT Department FROM Departments)

5. Sub query ใช้สำหรับ การ query data สามารถทำเป็น condition เพิ่มเติมได้ ก็จะ query ข้อมูลใหญ่ออกมาดู

Test