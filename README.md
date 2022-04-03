# # Capstone Project II - Files ##

# CONTENTS #

[Project Objectives](#Project-Objectives)

[Requirements and Installation](#Requirements-and-Installation)

[Application components](#Application-components)

[Contributors](#Contributors)

[License](#License)

# Project Objectives #

The purpose of this Capstone Project is to showcase my skills in handling input and output of external text files in Python. This project also forms part of my developer
portfolio. 

In this Capstone Project, I designed a task management application system to assist a small business in managing the tasks assigned to each user. The program works with
the following text files:
1. __user.txt__: This text file stores all the usernames and corresponding passwords of the user authenticated to use the program. 
2. __tasks.txt__: This text file contains data about the tasks assigned to each user, including the username to whom the task is assigned, assigned and due dates, 
   task title, task description, etc.

# Requirements and Installation #

In  order to *run and test* this program, you require the following:
- Python v3.7 or higher installed on your device
  - To download and install Python click the following link: *https://www.python.org/downloads/*

# Application components #
Open and run __task_manager.py__

### This task management system comprises the following sections of code:
# 1. User and password lists: #
  - all users and corresponding passwords contained in the user.txt file is appended to the user_list and password_list, respectively. 
  - 
# 2. Admin login and menu: #
  - A while loop is used to validate the user's login credentials. If the login credentials is recognised as "admin", then admin menu will be presented to the user. 
  - The admin menu has the following options:
    - r - Registering a user (register a new user) - new user login credentials will be written to __user.txt__
    - a - Adding a task (add a new task) - new task information will be written to __tasks.txt__
    - va - View all tasks (view all assigned tasks) - tasks will be read and displayed from __tasks_txt__
    - vm - View my task (view their own assigned tasks)
    - d - Display statistics (display user and task stats) 
    - e - Exit (exit the program)
  - Only admin users are authenticated to register new users and display statistics. 
  - 
  __Sample output for admin users__:
  ![admin_ouput1](https://user-images.githubusercontent.com/102178512/161425062-b318c284-8d3d-4212-b138-bdd1c91d17c0.jpg)
  ![admin_output2](https://user-images.githubusercontent.com/102178512/161425067-8a9941ba-ba7a-47b5-bd36-0e702f252cb2.jpg)
  
 # 3. User login and menu:
   - A while loop is used to validate the user's login credentials. If the user enters an invalid username or password, they will repeatedly be prompted 
     to enter valid login details. 
     
     __See sample error message for invalid login credentials:__
     ![invalid_login](https://user-images.githubusercontent.com/102178512/161425233-7cd9ad99-9207-4fef-baef-273d35aeb728.jpg)

   - Once other users have successfully logged in, they will see the following menu options:
     - a - Adding a task
     - va - View all tasks
     - vm - View my task
     - e - Exit
   - As seen above, other users have limited options compared to that of admin users. 
   - Should a user, other than an admin click "r" to register a new user, they will receive below __below sample error__ for not having appropriate 
     permission to do so:
   ![restricted_permissions](https://user-images.githubusercontent.com/102178512/161425464-8128f45f-1a58-4038-b0f2-d83e0feb7f92.jpg)
   
   __Sample output for other users__:
   ![vm_other_users](https://user-images.githubusercontent.com/102178512/161425589-8d345aea-c904-4264-9f07-d4013c460d80.jpg)
   
# Contributors
(c) Tammy-Lee Bastian tammyleebastian@gmail.com
   
# License
(c) Tammy-Lee C Bastian, HyperionDev
   
Licensed under the [MIT License](License)

