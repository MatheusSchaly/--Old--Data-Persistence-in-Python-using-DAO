# Data-Persistence-using-DAO

Using Data Access Object (DAO) pattern in Python to persist data both in a file as well as in a relational database. Three main modules were created:

1. I started using the Pickle library, so there will be a module named "student_dao_file_pickle" that will use Pickle to persist data in a txt file. But I didn't like how I implemented the "delete_student" method. Because I couldn't directly select the student that I wanted to delete, so I had to create a new txt file every time, which is not good. It was then that I discovered the Shelve library.

2. The Shelve library enabled me to store objects as in a dictionary. Therefore, I could retrieve the data that I wanted. Now, with Shelve, the delete method works much better. And you can notice the differences by checking the "student_dao_file_pickle" module and the "student_dao_file_shelve".

3. The third module named "student_dao_postgres" persists the data in a relational database. It was created to show the capability of DAO being able to, through a same interface "student_dao", persists the data in as many forms as you want.

I'm only a student, so don't take this repository too seriously. I did it all just to understand a little bit about data persistence in Python. Any suggestion is appreciated.
