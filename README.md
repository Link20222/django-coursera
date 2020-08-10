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
[Html Cheatsheet](https://github.com/Rustam-Z/django-coursera/blob/master/HTML_CHEAT_SHEET_PNG.png)
### Wekk 4 - CSS
[CSS Cheatsheet](http://www.lesliefranke.com/files/reference/csscheatsheet.html)
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
# COURSE 2
### Week 1 & 2
- Go to slides/course_2 
- MVC (Model-View-Controller) = MTV(Model-Template-View)
- ORM (Object Relational Mapper) 'models.py', it is easier to write the ORM then SQL code, u may have many DB
- Views
- Templates & Templates engine & Templates inheratance 
- Urls - URL mapping and reversing
- [Template tags and build-in filters](https://docs.djangoproject.com/en/3.0/ref/templates/builtins) 
- {% load foo bar from somelib%} -> csrf_token, block, url, include, extend, lorem, now, cycle, spaceless, or, and, not, in, for, if, endfor, endif
- {{value|lorem}} -> get_static_prefix, urlize, slugify, pluralize, wordcount, upper, lower, unordered_list, truncatewords, truncatechars, title (upper the first letter), capfirst, timeuntil, timesince, time, ljust, cetner, rjust, length, length_is, last, cut, add, 

### Week 3 
- OOP in Python
- [OOP concepts](https://www.py4e.com/html3/14-objects) 
- [Generic Display Views](https://docs.djangoproject.com/en/3.0/ref/class-based-views/generic-display/)
- ListView and DetailView

### Week 4 
- Forms, GET, POST, and HTTP
- GET for reading
- POSt for (saving, editing, deleting)
- CSRF Token (Cross site request forgery)
- Tip: Use {% 'csrf' token %} with POST, + use redirect
