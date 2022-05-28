
# Art Gallery Management System

This repository contains the complete code for making an *Art Gallery Management System*.

- *Language used for GUI:* Python (tkinter)
- *Language used for connectivity with the database:* Python (cx_Oracle)
- *Database used:* Oracle 21c

## About the project

On running the `.ipynb` file, a GUI window will pop up which looks like this:  
  
  
<img width="822" alt="artGal1" src="https://user-images.githubusercontent.com/92393664/170831256-175117c4-e3c1-4253-a429-1c8acc4d6170.png">

It has 5 tables in the database (2 tabs for each table - one to insert data and the other to display it) namely "exhibition", gallery"" "artist", "painting" and "customer". 
After inserting the data in a table, press the submit button. A "Record added in xyz table" message will pop up if the insertion was done successfully, otherwise an error message will be printed in the ouput window on jupyter notebook/IDE.  
  
<img width="825" alt="artGal2" src="https://user-images.githubusercontent.com/92393664/170831289-7444d4a6-0f52-4e4a-93dc-f0d4015e3507.png">  

Use the display tab to view all the entries in the respective table.  
  
<img width="818" alt="artGal3" src="https://user-images.githubusercontent.com/92393664/170831304-0e8e8f23-71f4-49f9-a190-ecaf1b86a944.png">  

## Steps to run

1. Make a new user in your database to simplify the maintenance of table data. 
2. Open the `galleryDB.sql` file in your database* and run the commands for table creation using the newly created user.
3. Open the `artGallery.ipynb` file with Jupyter Notebook (preferred) or any other python IDE.
4. Edit the part where connection to the database was made using `cx_Oracle`** according to your username and password and run the first cell to reach the GUI screen.
5. Now you can try entering and displaying the data entered in the tables.

\* *This repository uses Oracle as the database. You may use any other database, but in that case, you would need to make appropriate changes in the code.*  

\** *You may need to install cx_Oracle library and other libraries as well, like tkinter etc. You may check the imports at the top of the first cell in the `.ipynb` file and install them accordingly.*  

## References

https://docs.python.org/3/library/tk.html  
https://cx-oracle.readthedocs.io/en/latest/  
https://www.oracle.com/database/technologies/appdev/python/quickstartpythononprem.html  
