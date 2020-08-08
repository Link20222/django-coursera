# Django for Everybody
# COURSE 1
## PythonAnywhere: 
- https://help.pythonanywhere.com/pages/FollowingTheDjangoTutorial/
- https://www.dj4e.com/assn/dj4e_install.md
1. mkvirtualenv my_env --python=/usr/bin/python3.8
2. pip install django
3. git clone https://github.com/csev/dj4e-samples
4. cd dj4e-samples
5. pip install -r requirements.txt 
6. Database Handout - Command line SQLite
 - https://www.dj4e.com/lectures/SQL-01-Basics.txt
 - Start the command line in a Linux/Bash shell:
 - sqlite3 zip.sqlite3
 - Exit with ".quit", statements end with a semicolon.
 - .mode column
 - CREATE TABLE "Users" (
     "id" INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL UNIQUE, 
     "name" TEXT,
     "email" TEXT);
 - .tables
 - .schema Users
 - INSERT INTO Users (name, email) VALUES ('Kristen', 'kf@umich.edu');
 - SELECT * FROM Users;
 - DELETE FROM Users WHERE email='ted@umich.edu';
 - UPDATE Users SET name="Charles" WHERE email='csev@umich.edu';
 - SELECT * FROM Users WHERE email='csev@umich.edu';
 - SELECT * FROM Users ORDER BY email;
 - SELECT * FROM Users ORDER BY name DESC;
 - If you want: DROP TABLE Users 
 - .quit
