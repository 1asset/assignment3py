# Assignment3 SE-2004 (Dias Karibaev,Asset Kanatov,Yeskendir Iskakov)

Writing program to check user verification using Flask library.

## Installation
Before starting to use the code you must install required packages and modules. All packages and libraries will be provided in requirements.txt file, that is uploaded in the repository.

Pypi
bash
$ pip install requirements.txt

## Usage

At first we need to create a database in DBMS application(SQL server,Pgadmin) or other database management system. After that, you need to successfully connect your server with the database. We called our database "flask" as it is shown in the code. Also, it's important to know the login and password of your database, ours is postgres and 5432.

```  app.config['SQLALCHEMY_DATABASE_URI'] = 'postgresql://postgres:5432@localhost/flask' ```

The next step is to create a table in your new database, the database name is authorizationn.
``` CREATE TABLE authorization (
id INTEGER PRIMARY KEY, 
login VARCHAR,
password VARCHAR,
token VARCHAR
) 
```
Further step is to run users.py file, so it inserts the row into the table and after that you need to comment the last 4 rows in the code, because you already created a script. If you don't do that, you'll have an error, because it keeps creating the same script and the id is not distinct.
After these steps, you are ready to run test.py file. It is a main file and you'll get a link in the terminal, that you should follow.
```* Debugger is active!
* Debugger PIN: 989-466-843
* Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
```
