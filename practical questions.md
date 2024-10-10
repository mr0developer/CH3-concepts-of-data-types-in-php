### 1. Simple Program Using Constants

```php
<?php
// Define constants
define("EMPLOYEE_CODE", "001");
define("EMPLOYEE_NAME", "ABC");
define("EMPLOYEE_SALARY", 25000);
define("WORKING_HOURS", 7.5);

// Display the values
echo "Employee code is " . EMPLOYEE_CODE . "<br>";
echo "Employee Name is " . EMPLOYEE_NAME . "<br>";
echo "Employee Salary is " . EMPLOYEE_SALARY . "<br>";
echo "Working Hours are " . WORKING_HOURS . "<br>";
?>
```

### 2. Repeat the Above Program Using Variables

```php
<?php
// Define variables
$employeeCode = "001";
$employeeName = "ABC";
$employeeSalary = 25000;
$workingHours = 7.5;

// Display the values
echo "Employee code is " . $employeeCode . "<br>";
echo "Employee Name is " . $employeeName . "<br>";
echo "Employee Salary is " . $employeeSalary . "<br>";
echo "Working Hours are " . $workingHours . "<br>";
?>
```

### 3. How Do You Make a Constant Name Case Insensitive?

To make a constant name **case-insensitive**, you can pass a `true` value as the third argument to the `define()` function. By default, constant names are case-sensitive.

**Example:**
```php
<?php
define("GREETING", "Hello, World!", true);

// Both will work
echo GREETING;  // Outputs: Hello, World!
echo greeting;  // Outputs: Hello, World!
?>
```

### 4. How Do You Declare a Constant in PHP (With Example)?

In PHP, constants are declared using the `define()` function. Constants are used for values that will not change during the execution of the script.

**Syntax:**
```php
define("CONSTANT_NAME", value, case_insensitive);  // case_insensitive is optional
```

**Example:**
```php
<?php
define("SITE_URL", "https://www.example.com");

// Display the constant value
echo "Visit us at " . SITE_URL;
?>
```

### 5. Simple Program to Set Your G.R No. and Name in Variables and Display Using `echo` and `print`

```php
<?php
// Define variables
$grNo = "GR123456";
$name = "John Doe";

// Display using echo
echo "G.R No: " . $grNo . "<br>";
echo "Name: " . $name . "<br>";

// Display using print
print "G.R No: " . $grNo . "<br>";
print "Name: " . $name . "<br>";
?>
```

This program sets the G.R No. and name in variables and displays them using both `echo` and `print` functions.
