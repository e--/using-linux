mysql
============

mysql start command
------------------------
::

    mysql --help
    mysql -h localhost -u root -p
    select version(),current_date;
    select user();
    show databases;
    use mysql;
    show tables;
    create database demo;
    create user 'demo'@'%' identified by 'demo';
    grant all on demo.* to 'demo'@'%';
    flush privileges;

