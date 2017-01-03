# 基本概念

## 数据库 DB
Database, 数据的容器

## 数据库管理系统 DBMS
Database Management System，管理数据的软件。    
大部分所说的 MySQL、SQL Server、SQLite 都指的 DBMS    
PS：要搞清楚 「数据库」和「数据库管理系统」的区别

## 表 Table
某种特定类型数据的结构化清单

### 模式 Schema
关于数据库和表的布局及特性的信息描述。    
我们在创建一张表的时候，需要描述一张表的字段，字段类型，关系等信息的时候，这个叫做「模式」

## 行 Row
别称 记录 Record。    
指的表中的一个记录

## 键 Key

### 主键 Primary Key
一列能够唯一标识表中每一行。    
特性：    
1. 唯一    
2. 非空    
3. 不予修改和更新    

### 联合主键 Union Primary Key
多个列组合成的主键    
所有列值得组合符合「主键」的特性

### 外键
链接一个表和另外一个表的钩子，外键往往是另外一个表的主键

## SQL
Structured Query Language    
SQL是有标准的，标准版的SQL：[ANSI SQL](https://www.wikiwand.com/zh-hans/SQL)    
各个DBMS厂商都在支持标准的SQL基础上，根据自身功能扩展SQL。这也是SQL移植性很差的原因之一。    
特性：    
1. 不分大小写    
2. 语句结尾分号没有必要性（MySQL强制加上）    
3. 空格会被忽略，一条语句可以分多行，也可以一行    

## 子句 Clause
SQL语句由子句构成，有些子句是必须的，有些则是可选的。    
一个子句通常由一个关键字加上所提供的数据组成，如：    
1. SELET filed1_name, filed2_name    
2. FROM table_name    
3. ORDER BY filed_name    

SELECT 的子句有：    

* SELECT    
* FROM    
* WHERE    
* GROUP BY    
* HAVING    
* ORDER BY    