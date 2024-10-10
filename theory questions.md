### 1. What is the difference between Variables and Constants?

- **Variables**:
  - Variables are containers for storing data values that **can change** during the execution of a program.
  - In PHP, variables are declared using the `$` symbol followed by a name (e.g., `$name = "John";`).
  - Example:  
    ```php
    $age = 25;
    $age = 30; // Variable value can be changed
    ```

- **Constants**:
  - Constants hold **fixed values** that **cannot change** once they are defined during script execution.
  - Constants are declared using the `define()` function or the `const` keyword, and they do not use the `$` symbol.
  - Example:  
    ```php
    define("PI", 3.14159); // Using define() function
    const VERSION = "1.0.0"; // Using const keyword
    // These values cannot be changed later in the script.
    ```


---

### 2. Name and Describe the Four Data Types in PHP

The four primary data types in PHP are:

1. **String**:
   - A string is a sequence of characters enclosed in quotes (either single `' '` or double `" "`).
   - Example:  
     ```php
     $name = "John Doe";
     ```

2. **Integer**:
   - Integers are non-decimal whole numbers (positive or negative).
   - Example:  
     ```php
     $age = 25;
     ```

3. **Float (Double)**:
   - Floats are numbers that contain a decimal point or are expressed in exponential form.
   - Example:  
     ```php
     $price = 19.99;
     ```

4. **Boolean**:
   - Booleans represent two possible values: `true` or `false`.
   - Example:  
     ```php
     $is_active = true;
     ```

---

### 3. Explain the Purpose of the NULL Data Type

The **NULL** data type represents a variable with no value assigned. It is used when a variable is explicitly set to have no value or when a variable has not been initialized. In PHP, a variable is considered `NULL` if:
- It has been assigned the constant `NULL`.
- It has been declared but has not yet been assigned any value.
- It has been unset using `unset()`.

Example:
```php
$var = NULL;
if ($var === NULL) {
    echo "The variable is NULL.";
}
```

**Purpose**: NULL is useful for denoting empty, unset, or non-existent values in programs.

---

### 4. What Do You Mean by Strongly and Loosely Typed Programming?

- **Strongly Typed Programming**:
  - In strongly typed languages, data types are **strictly enforced**. This means that variables must be declared with a specific data type, and conversions between incompatible types often require explicit type casting.
  - Example: In Java, assigning a string to an integer variable would result in a compile-time error.

- **Loosely Typed Programming**:
  - In loosely typed languages, data types are **not strictly enforced**. PHP is loosely typed, which means that variables can change types dynamically, and the language automatically handles type conversions as needed.
  - Example: In PHP, you can assign an integer to a variable, and later assign a string to the same variable without an error.
    ```php
    $var = 10;   // Integer
    $var = "10"; // Now a string
    ```

---

### 5. What is Concatenation?

**Concatenation** is the process of combining or joining two or more strings together. In PHP, the dot (`.`) operator is used to concatenate strings.

Example:
```php
$firstName = "John";
$lastName = "Doe";
$fullName = $firstName . " " . $lastName;
echo $fullName; // Output: John Doe
```

In this example, the two strings `$firstName` and `$lastName` are concatenated with a space in between. The result is stored in `$fullName`.
