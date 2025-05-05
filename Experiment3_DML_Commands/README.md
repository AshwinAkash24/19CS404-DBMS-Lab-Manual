# Experiment 3: DML Commands
# Name: Ashwin Akash M
# Reference Number:212223230024
## AIM
To study and implement DML (Data Manipulation Language) commands.

## THEORY

### 1. INSERT INTO
Used to add records into a relation.
These are three type of INSERT INTO queries which are as
A)Inserting a single record
**Syntax (Single Row):**
```sql
INSERT INTO table_name (field_1, field_2, ...) VALUES (value_1, value_2, ...);
```
**Syntax (Multiple Rows):**
```sql
INSERT INTO table_name (field_1, field_2, ...) VALUES
(value_1, value_2, ...),
(value_3, value_4, ...);
```
**Syntax (Insert from another table):**
```sql
INSERT INTO table_name SELECT * FROM other_table WHERE condition;
```
### 2. UPDATE
Used to modify records in a relation.
Syntax:
```sql
UPDATE table_name SET column1 = value1, column2 = value2 WHERE condition;
```
### 3. DELETE
Used to delete records from a relation.
**Syntax (All rows):**
```sql
DELETE FROM table_name;
```
**Syntax (Specific condition):**
```sql
DELETE FROM table_name WHERE condition;
```
### 4. SELECT
Used to retrieve records from a table.
**Syntax:**
```sql
SELECT column1, column2 FROM table_name WHERE condition;
```
**Question 1**
--
Decrease the reorder level by 30 percent where the product name contains 'cream' and quantity in stock is higher than reorder level in the products table.

```sql
UPDATE products
SET reorder_lvl=reorder_lvl*0.70
WHERE product_name LIKE '%cream%' AND quantity>reorder_lvl;
```

**Output:**
![image](https://github.com/user-attachments/assets/90cb362e-0ae4-4353-bedd-73d015be70a6)


**Question 2**
---
 Update the total selling price to quantity sold multiplied by updated selling price per unit where product id is 10 in the sales table.

```sql
UPDATE SALES
SET total_sell_price=sell_price*quantity
WHERE product_id=10;
```

**Output:**
![image](https://github.com/user-attachments/assets/a2eeacc0-c578-4681-93f7-6a146ae62081)

**Question 3**
---
Write a SQL statement to Increase the salary by 500 and email as 'updated' for employees with job ID 'SA_REP' and commission percentage greater than 0.15

```sql
UPDATE Employees
SET salary=salary+500,email='updated' 
WHERE job_id='SA_REP' AND commission_pct>0.15;
```

**Output:**
![image](https://github.com/user-attachments/assets/eef00047-b4fa-40da-9b4c-002d21cf58f5)

**Question 4**
---
Write a SQL statement to change the email column of employees table with 'Unavailable' for all employees in employees table.

```sql
UPDATE employees
SET email='Unavailable';
```

**Output:**

![image](https://github.com/user-attachments/assets/43a75def-6e1a-4042-bebb-b0b4339de87c)

**Question 5**
---
Write a SQL statement to Change the category to 'Household' where product name contains 'Detergent' in the products table.
```sql
UPDATE Products
SET category='Household'
WHERE product_name LIKE '%Detergent%';
```

**Output:**
![image](https://github.com/user-attachments/assets/b73b8775-4d1b-4cb6-8206-b230b8e275b9)


**Question 6**
---
Write a SQL query to Delete All Doctors with a NULL Specialization

Sample table: Doctors

attributes : doctor_id, first_name, last_name, specialization

```sql
DELETE FROM Doctors
WHERE specialization IS NULL;
```

**Output:**
![image](https://github.com/user-attachments/assets/9d918d71-5227-42c3-b874-596e5d9cf5b0)


**Question 7**
---
Write a SQL query to Delete All Doctors whose ID ranges from 2 to 4.

Sample table: Doctors

attributes : doctor_id, first_name, last_name, specialization

```sql
DELETE FROM Doctors
WHERE doctor_id BETWEEN 2 AND 4;
```

**Output:**
![image](https://github.com/user-attachments/assets/95e822f5-e3ce-44e1-8ba1-35fdb654aa60)


**Question 8**
---
Write a SQL query to remove rows from the table 'customer' with the following condition -

1. 'cust_country' must be 'India',

2. 'cus_city' must not be 'Chennai',

```sql
DELETE FROM customer
WHERE CUST_COUNTRY='India' AND CUST_CITY!='Chennai';
```

**Output:**
![image](https://github.com/user-attachments/assets/d6b4356d-2e6c-47ef-9497-d6bd44fbba1f)

**Question 9**
---
Write a SQL query to delete a doctor from Doctors table whose Specialization is 'Pediatrics' and First name is 'Michael'.

Sample table: Doctors

attributes : doctor_id, first_name, last_name, specialization

```sql
DELETE FROM Doctors
WHERE specialization='Pediatrics' AND first_name LIKE 'Michael%';
```

**Output:**
![image](https://github.com/user-attachments/assets/69baf3f4-04f8-4b5c-9b1f-fa20e2fe9be4)


**Question 10**
---
Write a SQL query to Delete a Specific Surgery whose ID is 3 or surgeon ID is 4.
```sql
DELETE FROM Surgeries
WHERE surgery_id=3 OR surgery_id=4;
```

**Output:**
![image](https://github.com/user-attachments/assets/f8038ae7-8d9a-46d7-b01e-1ed9489134a1)


## RESULT
Thus, the SQL queries to implement DML commands have been executed successfully.
