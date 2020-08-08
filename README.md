# Django for Everybody Specialization 
# COURSE 1
### Week 1
- About Web sockets, Http, how the servers are working
- Building own broswer, server, web client in Python 

### Week 2 - PythonAnywhere: 
- https://help.pythonanywhere.com/pages/FollowingTheDjangoTutorial/
- https://www.dj4e.com/assn/dj4e_install.md

``` bash
mkvirtualenv my_env --python=/usr/bin/python3.8
pip install django
git clone https://github.com/csev/dj4e-samples
cd dj4e-samples
pip install -r requirements.txt 
```
### Week 3 - Html
### Wekk 4 - CSS
### Week 5 - Database Handout - Command line SQLite
- https://www.dj4e.com/lectures/SQL-01-Basics.txt
- Start the command line in a Linux/Bash shell:
``` bash
sqlite3 zip.sqlite3
.mode column
CREATE TABLE "Users" (
     "id" INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL UNIQUE, 
     "name" TEXT,
     "email" TEXT
);
.tables
.schema Users
INSERT INTO Users (name, email) VALUES ('Kristen', 'kf@umich.edu');
SELECT * FROM Users;
DELETE FROM Users WHERE email='ted@umich.edu';
UPDATE Users SET name="Charles" WHERE email='csev@umich.edu';
SELECT * FROM Users WHERE email='csev@umich.edu';
SELECT * FROM Users ORDER BY email;
SELECT * FROM Users ORDER BY name DESC;
# If you want: DROP TABLE Users 
.quit
```

