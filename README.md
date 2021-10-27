# Assignment3 SE-2004 (Dias Karibaev,Asset Kanatov,Yeskendir Iskakov)

Writing program to check user verification using Flask library

## Installation
Before starting to use the code you must install required packages and modules. All packages and libraries will be provided in requirements.txt file.

Pypi
bash
$ pip install requirements.txt

## Usage

At first we need to create a database in DBMS application(SQL server,Pgadmin) or other database management system. After that, you need to successfully connect your server with the database. We called our database "flask" as it is shown in the code. Also, it's important to know the login and password of your database, ours is postgres and 5432.

```  app.config['SQLALCHEMY_DATABASE_URI'] = 'postgresql://postgres:5432@localhost/flask' ```
