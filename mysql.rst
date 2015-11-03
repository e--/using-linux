mysql
============

mysql basic command
------------------------
login

.. code-block:: sql

    mysql --help
    mysql -h localhost -u root -p

info

.. code-block:: sql

    select version(),current_date;
    select user();
    show databases;
    use mysql;
    show tables;

create user

.. code-block:: sql

    create database demo;
    create user 'demo'@'%' identified by 'demo';
    grant all on demo.* to 'demo'@'%';
    flush privileges;


python connector
----------------------
connect code examples::

    import mysql.connector
    cnx=mysql.connector.connect(user='demo',password='demo',host='localhost',database='demo')
    c=cnx.cursor()
    c.execute('show tables')
    c.fetchall()
    c.close()
    cnx.close()



