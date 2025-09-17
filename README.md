# Week03 Quiz1:


## 1. Requirements:

Design an employee management program to support staff entry and query functions.

- Writing code using c++

### Input
- The first line contains a number (int type) representing the number of employees that are about to be entered.
- Starting from the second line, input the corresponding number of employee information based on the numbers entered in the first line. Format as `Name(string/char[] Type) Age(int Type) Salary(int Type) PhoneNumber(string/char[] Type)`, separated by spaces. Enter a new line for each employee's information until all input is complete. (Assuming the input is completely correct, fault handling is not considered for input error types.) 
- After entering the next line of all employee information, enter a number(int type) representing the times of searching commands to be executed next.
- Starting from the next line, input the corresponding number of query commands based on the numbers from the previous line. Format as `command_type(string/char type) query_conditions(string/char[] type if queried by name/phone number, int type if queried by age/monthly salary)`, use spaces separating the contents. Every command is followed by a new line until all inputs are complete.

#### Searching content and format:

- Search by name: `'n' name`. Among these, 'n' is a fixed letter, and 'name' is the name to be queried.
- Search by age: `'a' age`. Among these, 'a' is a fixed letter, and 'age' is the age to be queried.
- Search by salary: `'s' salary.` Among these, 's' is a fixed letter, and "salary" is the salary to be queried.
- Search by phone number: `'p' phoneNumber`. Among these, 'p' is a fixed letter, and 'phoneNumber' is the phone number to be queried.

### Output
- For every searching command input, the corresponding employee information is output. 
- When multiple pieces of information match, output each piece of information one by one, with a new line for each employee's information.
- When there is no matching employee information, output: `No such person.` 
- When the query command is entered incorrectly, output: `Error: Wrong order word!`。



## 2. Scoring Criteria (Total 5 points):

- No compilation error: 1 point
- Output is correct: 2 point
- Exception handling (when command input is incorrect): 2 point


## 3. Example: (Red font for input, blue font for output)

![image](https://github.com/chyh001228/images/blob/main/w3q1.png)

**Input:**

```
6
chominguk 30 17000 010-2214-3357
parkminguk 45 4000 010-5325-9400
parkminsu 42 13000 010-2179-8841
kimjiwon 56 7000 010-3456-7890
kimjihye 59 17000 010-1333-3333
parkcheolsu 44 7000 010-2436-8847
5
n parkminguk
p 010-3456-7890
s 7000
a 69
z chominguk
```

**Output:**

```
parkminguk 45 4000 010-5325-9400
kimjiwon 56 7000 010-3456-7890
kimjiwon 56 7000 010-3456-7890
parkcheolsu 44 7000 010-2436-8847
No such person.
Error: Wrong order word!
```

**Actual results:**
![image](https://github.com/chyh001228/images/blob/main/w3q1_c.png)


<img src="https://cdn.imweb.me/upload/S201906178853c3e170808/c5d876d707352.jpg" width=30% align=center />
