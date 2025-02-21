# **Understanding String Methods in Smart Task Manager**

## **📌 Overview**
Strings are widely used in **Smart Task Manager**, and various **built-in Java String methods** are applied to manipulate and validate text data. This document provides **detailed explanations** of each string method used in the project, its purpose, and expected output.

---

## **1️⃣ Commonly Used String Methods and Their Purpose**

### **🔹 `.trim()` – Remove Whitespace**
📌 **Purpose:** Removes leading and trailing spaces from a string.
```java
String input = "  Task Manager  ";
String trimmed = input.trim();
System.out.println(trimmed);
```
✔ **Expected Output:**
```plaintext
Task Manager
```
✔ **Explanation:**
- `.trim()` ensures that **extra spaces at the beginning and end** of a string are removed.
- Useful for **cleaning user input** before storing or processing it.

---

### **🔹 `.equals(String)` – Compare Strings for Equality**
📌 **Purpose:** Checks whether **two strings are exactly the same** (case-sensitive).
```java
String status = "COMPLETED";
if (status.equals("COMPLETED")) {
    System.out.println("Task is completed!");
}
```
✔ **Expected Output:**
```plaintext
Task is completed!
```
✔ **Explanation:**
- Returns `true` if both strings **match exactly**.
- **Case-sensitive**, meaning `"completed".equals("COMPLETED")` would return `false`.

---

### **🔹 `.equalsIgnoreCase(String)` – Compare Strings (Ignore Case)**
📌 **Purpose:** Compares strings without considering **uppercase and lowercase differences**.
```java
String priority = "High";
if (priority.equalsIgnoreCase("high")) {
    System.out.println("Task has high priority!");
}
```
✔ **Expected Output:**
```plaintext
Task has high priority!
```
✔ **Explanation:**
- This method **ignores case**, so `"HIGH"` and `"high"` are treated as equal.
- Useful for **case-insensitive comparisons**, such as user inputs.

---

### **🔹 `.contains(String)` – Check if a String Contains a Substring**
📌 **Purpose:** Determines if a string contains **a specific sequence of characters**.
```java
String taskDescription = "Finish Java project";
if (taskDescription.contains("Java")) {
    System.out.println("This task is related to Java!");
}
```
✔ **Expected Output:**
```plaintext
This task is related to Java!
```
✔ **Explanation:**
- Returns `true` if the given substring **exists inside** the main string.
- **Case-sensitive**, meaning `"java"` would **not** match `"Java"`.

---

### **🔹 `.startsWith(String)` – Check String Prefix**
📌 **Purpose:** Checks if a string **begins** with a certain sequence of characters.
```java
String filename = "task_list.txt";
if (filename.startsWith("task")) {
    System.out.println("This file contains task information.");
}
```
✔ **Expected Output:**
```plaintext
This file contains task information.
```
✔ **Explanation:**
- Returns `true` if the string **starts with** the given sequence.
- Useful for **checking filename formats** or input validation.

---

### **🔹 `.endsWith(String)` – Check String Suffix**
📌 **Purpose:** Checks if a string **ends** with a certain sequence of characters.
```java
String filename = "document.pdf";
if (filename.endsWith(".pdf")) {
    System.out.println("This is a PDF file.");
}
```
✔ **Expected Output:**
```plaintext
This is a PDF file.
```
✔ **Explanation:**
- Returns `true` if the string **ends with** the given suffix.
- Commonly used for **file type validation**.

---

### **🔹 `.replace(String target, String replacement)` – Replace Characters**
📌 **Purpose:** Replaces **all occurrences** of a substring within a string.
```java
String message = "Hello, User!";
String updatedMessage = message.replace("User", "Carmel");
System.out.println(updatedMessage);
```
✔ **Expected Output:**
```plaintext
Hello, Carmel!
```
✔ **Explanation:**
- Replaces **all** instances of the target substring.
- Useful for **customizing messages dynamically**.

---

### **🔹 `.toLowerCase()` and `.toUpperCase()` – Change Case**
📌 **Purpose:** Converts a string to **all lowercase** or **all uppercase**.
```java
String input = "Java Programming";
System.out.println(input.toLowerCase());
System.out.println(input.toUpperCase());
```
✔ **Expected Output:**
```plaintext
java programming
JAVA PROGRAMMING
```
✔ **Explanation:**
- `.toLowerCase()` changes all characters to **lowercase**.
- `.toUpperCase()` changes all characters to **uppercase**.
- Often used for **normalizing user input before comparisons**.

---

## **🚀 Summary**
✔ **trim()** – Removes leading/trailing spaces.  
✔ **equals()** – Checks if two strings are **exactly** the same (case-sensitive).  
✔ **equalsIgnoreCase()** – Compares two strings **without case sensitivity**.  
✔ **contains()** – Checks if a string **contains** a given substring.  
✔ **startsWith() / endsWith()** – Checks if a string **starts or ends** with a given value.  
✔ **replace()** – Replaces occurrences of **one substring** with another.  
✔ **toLowerCase() / toUpperCase()** – Converts a string to **lowercase or uppercase**.

By understanding these **string methods**, you can write more efficient and readable Java code! 🚀

