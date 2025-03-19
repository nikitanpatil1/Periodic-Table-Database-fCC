# Periodic Table Database

*This project consists of creating a Bash script to get information about chemical elements from a periodic table database.*

## Problem Statement

You are started with a periodic_table database that has information about some chemical elements. Read the instructions below and complete user stories to finish the project:

### Part 1: Fix the database 

  There are some mistakes in the database that need to be fixed or changed. See the user stories below for what to change:
  
  - Rename the *weight* column to **atomic_mass**. Rename the *melting point* column to **melting_point_celsius** and the *boiling_point* column to **boiling_point_celsius**.
  - *melting_ point_celsius* and *boiling_point_celsius* columns should not accept **null** values.
  - Add the **UNIQUE** constraint to the *symbol* and *name* columns from the elements table. The *symbol* and *name* columns should have the **NOT NULL** constraint.
  - Set the *atomic _number* column from the *properties* table as a foreign key that references the column of the same name in the *elements* table.
  - Create a **types** table that will store the three types of elements. The *types* table should have a **type_id** column that is an **integer** and the primary key. The *types* table should have a **type** column that's a **VARCHAR** and cannot be **null**. It will store the different types from the **type** column in the *properties* table. Add three rows to The *types* table whose values are the three different types from the *properties* table.
  - The *properties* table should have a **type_id** foreign key column that references the **type_id** column from the *types* table. It should be an **INT** with the **NOT NULL** constraint. Each row in the *properties* table should have a **type_id** value that links to the correct **type** from the *types* table.
  - Capitalize the first letter of all the **symbol** values in the *elements* table. Be careful to only capitalize the letter and not change any others.
  - Remove all the trailing zeros after the decimals from each row of the *atomic_mass* column. You may need to adjust a data type to **DECIMAL** for this. The final values they should be are in the *atomic_mass.txt* file 
  - Add the element with atomic number 9 to the database. Its name is Fluorine, symbol is F, mass is 18.998, melting point is -228, boiling point is -188.1, and it's a nonmetal. Add the element with atomic number 10 to the database. Its name is Neon, symbol is Ne, mass is 20.18, melting point is -248.6, boiling point is -246.1 and it's a nonmetal.
  - Delete the non existent element, whose atomic_number is 1000, from the two tables.
  - The properties table should not have a *type* column. 

### Part 2: Create your git repository

  Make a small bash program. The code needs to be version controlled with git, so you will need to turn the suggested folder into a git repository. 
  
  - Create a **periodic_table** folder in the *project* folder and turn it into a git repository with **git init**.
  - The repository should have a **main** branch with all the commits. The **periodic_table** repo should have at least five commits.
  - Finish the project while on the main branch. The working tree should be clean and should not have any uncommitted changes.

### Part 3: Create the script

  Make a script that accepts an argument in the form of an "atomic number", "symbol", or "name" of an element and outputs some information about the given element.
  
  - Create an **element.sh** file in the repo folder. 
  - If user run **./element.sh**, it should output only "*Please provide an element as an argument.*" and finish running.
  - If user run **./element.sh 1**, **./element.sh H**, or **./element.sh Hydrogen**, it should output only "*The element with atomic number 1 is Hydrogen (H). It's a nonmetal, with a mass of 1.008 amu. Hydrogen has a melting point of -259.1 celsius and a boiling point of -252.9 celsius.*" 
  - If user run **./element.sh** script with another element as input, it should get the same output but with information associated with the given element.
  - If the argument input to the **element.sh** script doesn't exist as an "atomic_ number", "symbol", or "name" in the database, the only output should be "*I could not find that element in the database.*"

### fix database 
![Image](https://github.com/user-attachments/assets/a7b0765c-28eb-4b66-9ab4-8823590eb61e)

![Image](https://github.com/user-attachments/assets/c4f18511-3595-4b65-a530-16da367c68a9)

![Image](https://github.com/user-attachments/assets/b1f5a7cc-de96-4bf9-9cc2-b21641a81d8e)

![Image](https://github.com/user-attachments/assets/35db1375-7d73-4da2-b9a3-f1cda526feb1)

![Image](https://github.com/user-attachments/assets/b52e66b5-5998-496e-a134-cbba32ce03ac)

![Image](https://github.com/user-attachments/assets/adcbdfe1-8842-44f9-be37-7cd04155e4f1)

![Image](https://github.com/user-attachments/assets/dd869058-6ba6-45ff-8d5e-3b34983a559e)

![Image](https://github.com/user-attachments/assets/3963f579-a69e-4f6a-b348-60eac5d4388f)

![Image](https://github.com/user-attachments/assets/5b0a6037-ba8b-466f-a517-3da64a86a443)

![Image](https://github.com/user-attachments/assets/d15b6794-f7fd-468d-849f-124a35a8681a)

![Image](https://github.com/user-attachments/assets/14dba789-a195-4e70-9e9b-b41782ed01ed)

![Image](https://github.com/user-attachments/assets/f26a445c-46a6-4d67-84d6-dd13b00d6049)

![Image](https://github.com/user-attachments/assets/7ce85ca1-805d-457b-8f3d-617111abbe18)

![Image](https://github.com/user-attachments/assets/18c36201-36a2-4409-88f2-20c8ec833cad)

### final output
