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

![Image](https://github.com/user-attachments/assets/b1aafa19-fd71-48a5-b1f0-14debfe1ea09)

![Image](https://github.com/user-attachments/assets/11b9f1ea-d422-4cc7-bca4-7f0e2a3e90fd)

![Image](https://github.com/user-attachments/assets/08d3201b-7be4-48ff-980c-3c74acce4380)

![Image](https://github.com/user-attachments/assets/54061de1-c13c-4330-84ba-10c432525c8d)

![Image](https://github.com/user-attachments/assets/98a7094b-695a-487d-9dc8-f3e90663d430)

![Image](https://github.com/user-attachments/assets/65f2301e-f145-49d6-832f-c94c4af2a551)

![Image](https://github.com/user-attachments/assets/7940efff-f7ac-4dd3-b930-de1b5c4ff69d)

![Image](https://github.com/user-attachments/assets/9ceff4a8-89db-49b6-94cb-e81d917096c1)

![Image](https://github.com/user-attachments/assets/183d4c7f-2fcf-4e50-8bce-d4ee29ce1045)

![Image](https://github.com/user-attachments/assets/61a8c8f3-5553-4c3a-b297-6324630bcfed)

![Image](https://github.com/user-attachments/assets/39131342-91ee-47e1-9f8b-6d6fa4acc43b)
