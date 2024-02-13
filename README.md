# **Printf Function**
<p align="center">
  <img src="SimpleShellBanner.gif" width="650" height="200">
</p>

## **📋 Table of Contents**
1. [Introduction](#introduction)
2. [Synopsis](#synopsis)
3. [Project](#Project)
  - [General Requirements](#general-requirements)
  - [Functions and system calls used](#functions-and-system-calls-used)
    - [Description of each file](#description-of-each-file)
  - [Environment](#environment)
  - [Compilation](#compilation)
  - [Testing](#testing)
    - [Interactive](#interactive-mode)
    - [Non-Interactive](#non-interactive-mode)
    - [Sample usage](#sample-usage)
    - [Stop and return to your original shell](#stop-and-return-to-your-original-shell)
  - [Project Tasks](#project-tasks)
5. [Authors](#authors)

## **📜Introduction**
 * In this project we coded from scratch a simple Unix printf function.
  
  * But what is a printf function?
    
    Printf is a standard output formatting function commonly found in programming languages such as C, C++, and other related languages. The name "printf" stands for "print formatted," and its primary purpose is to produce formatted output based on a specified format string.
    
[Back to Top](#project-name)
    
## **💡Synopsis**

  This repository holds all the code necessary for our custom printf function to run. Our printf currently handles the input is receiving to return an output and prints it
  
[Back to Top](#project-name)
  
## **💽Project**

### **📑General Requirements**
  
  - Allowed editors: `vi`, `vim`, `emacs`
  - All the files should end with a new line
  - A `README.md` file, at the root of the folder of the project is mandatory
  - The shell should not have any memory leaks
  - No more than 5 functions per file
  - All the header files should be include guarded
  - The se system calls should be only when needed to

### **💻Functions and system calls used**

  
#### **🗃Description of each file**

<!DOCTYPE html>
<html>

  <body>

<table style="width:100%">
  <tr>
    <th>File Name</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><a href="https://github.com/jGohan-cpu/holbertonschool-simple_shell/blob/master/main.c">main.c</a></td>
    <td>Main function that run the shell</td>  
  </tr>
  <tr>
    <td><a href="https://github.com/jGohan-cpu/holbertonschool-simple_shell/blob/master/execute.c">execute.c</a></td>
    <td>Responsible to for executing the command given</td>
  </tr>
  <tr>
    <td><a href="https://github.com/jGohan-cpu/holbertonschool-simple_shell/blob/master/prompt.c">prompt.c</a></td>
    <td>Function which prints the shell prompt symbol ($)</td>
  </tr>
  <tr>
    <td><a href="https://github.com/jGohan-cpu/holbertonschool-simple_shell/blob/master/read_line.c">read_line.c</a></td>
    <td>Function that read a line of input from the user</td>
  </tr>
  <tr>
    <td><a href="https://github.com/jGohan-cpu/holbertonschool-simple_shell/blob/master/tokens.c">tokens.c</a></td>
    <td>Takes user input and splits it into and array of arguments</td>
  </tr>
  </tr>
  <tr>
    <td><a href="https://github.com/jGohan-cpu/holbertonschool-simple_shell/blob/master/env.c">env.c</a></td>
    <td>Handles the environmetal varibles</td>
  </tr>
  <tr>
    <td><a href="https://github.com/jGohan-cpu/holbertonschool-simple_shell/blob/master/shell.h">shell.h</a></td>
    <td>Header file with prototypes and header files required for the program</td>
  </tr>
  <tr>
    <td><a href="https://github.com/jGohan-cpu/holbertonschool-simple_shell/blob/master/man_1_simple_shell">man_1_simple_shell</a></td>
    <td>Simple man page of our shell</td>
  </tr>
  <tr>
    <td><a href="https://github.com/jGohan-cpu/holbertonschool-simple_shell/blob/master/AUTHORS">Authors</a></td>
    <td>Names of the authors of the project</td>
  </tr>
</table>

</body>
</html>




### **🌎Environment**
  - Language: C
  - OS: Ubuntu 20.04
  - Compiler: gcc
  - Style guideines: Betty Style

### **💻Compilation**
  - All of our files will be compiled using:

    `gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh`
    
  
### **💻Testing**
  
   -You can test our custom version of the shel in the interactive and non-interactive mode.
    
#### **💻Interactive mode**

  - The shell should work like this in interactive mode:
    
  ```bash
  $ ./hsh
  ($) /bin/ls
  hsh main.c shell.c
  ($)
  ($) exit
  $
  ```
    
#### **💻Non-Interactive mode**

  -In the non-interactive mode should work like this:
  
      
    $ echo "/bin/ls" | ./hsh
    hsh main.c shell.c test_ls_2
    $
    $ cat test_ls_2
    /bin/ls
    /bin/ls
    $
    $ cat test_ls_2 | ./hsh
    hsh main.c shell.c test_ls_2
    hsh main.c shell.c test_ls_2
    $
    

#### **💻Sample usage**

  - This is a simple example of what and how can you do some commands in our custom shell:
    
    ```bash
    $ echo "This is a pretty cool!"
    This is pretty cool!
    $ man ./man_1_simple_shell (opens our manpage for more information)
    ```

#### **💻Stop and return to your original shell**

  - To stop our shell and return to your original shell you should type the command:
    
    ```bash
    $ exit
    (your_terminal)$
    ```
    
[Back to Top](#project-name)
  
    
-Task 0
  -Write a README:
  -Write a man for your printf function:
  -Create a manual page (man) that explains the usage and features of your printf function.
  -Include information on supported format specifiers and any specific options.
  -AUTHORS file:

-Task 1
  -Write beautiful code that passes Betty checks:
  -Refactor your printf function code to adhere to the Betty coding style.
  -Ensure proper indentation, spacing, and variable/function naming conventions.
  
-Task 2
  -Write a printf function:
  -Implement a basic version of the printf function.
  -Display the formatted output based on the provided format specifiers.
-Task 3
  -Handle printf function with arguments:
  -Modify the printf function to accept variable arguments and format them accordingly.
  -Ensure proper handling of different data types and format specifiers.
-Task 4
  -Handle printf function with PATH:
  -Modify the printf function to incorporate the PATH for any additional formatting or information.
  -Ensure the printf function behaves appropriately when the specified format requires external data.
-Task 5
  -Implement the exit built-in for printf:
  -Create a function that exits the program when the printf function encounters a specified exit condition.
  -Ensure it does not take any arguments.
-Task 6
  -Implement the env built-in for printf a function that prints the current environment using the printf function.
  -Display relevant environment information with proper formatting.

[Back to Top](#project-name)

## 🤝Authors
![Jose Rivera](https://github.com/jGohan-cpu)
![Jean Barbosa](https://github.com/JeanBarbosa-hue)

[Back to Top](#project-name)
