Project: Nile Dot Com (Event-Driven Programming)
Author: Joshua Jaggernauth
Course: CNT 4714 – Fall 2025
Date: September 7, 2025

---------------------------------
Contents of Project1_NileDotCom:
---------------------------------
This folder contains all required deliverables for Project 1:
- A subfolder with the required screenshots
- The transactions.csv file generated after running the application
- A zip archive containing all Java source files (CSVLoader.java, InventoryItem.java, NileStoreApp.java),
  the inventory.csv input file, and other supporting files

Together, this demonstrates that I have included all required materials.

--------------------
How to Run the Code:
--------------------
In Eclipse:
1) Import the provided zip archive (File → Import → Existing Projects into Workspace → Select archive file).
2) Run NileStoreApp.java as a Java Application.
3) Ensure inventory.csv is at the project root (same level as src/).
4) Interact with the GUI: Find → Add → Checkout. transactions.csv will update after each checkout.

From the command line:
1) Extract the source zip to a folder.
2) Navigate to the project root in a terminal.
3) Compile: javac -d out src/estore/*.java
4) Run: java -cp out estore.NileStoreApp

----------------
Implementation:
----------------
- Look & Feel: Nimbus (built into Java; no external libraries required).
- transactions.csv is generated and appended with each checkout.
- Each transaction can hold up to 5 items.
- Discounts applied: 5–9 items = 10%, 10–14 = 15%, 15+ = 20%.
- After checkout, an invoice is displayed and the order is locked.
- New Order starts another transaction; Exit closes the application.
