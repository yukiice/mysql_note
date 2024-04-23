## 1、SQL分类

- DDL
  - 数据定义语言，用于定义数据库对象(数据库、表、字段)
- DML
  - 数据操作语言，用于对数据库表中的数据进行增删改
- DQL
  - 数据查询语言，用于查询数据库中表的记录
- DCL
  - 数据控制语言，用来创建数据库用户、控制数据库的访问权限



### 1.DDL

---

#### 1.DATABASE

- 查询

  - 查询所有数据库

    - ```sql
      SHOW DATABASES;
      ```

  - 查询当前所选择的数据库

    - ```
      SELECT DATABASE();
      ```

  - 创建数据库

    - ```
      CREATE DATABASE [IF NOT EXISTS] 数据库名 [DEFAULT CHARSET字符集] [COLLATE排序规则]
      ```

  - 删除数据库

    - ```
      DROP IF EXISTS 数据库名
      ```

  - 使用数据库

    - ```
      USE 数据库名
      ```



#### 2.TABLE

- 查询当前数据库所有表

  - ```
    SHOW TABLES;
    ```

- 查询表结构

  - ```
    DESC 表名
    ```

- 查询指定表的建表语句

  - ```
    SHOW CREATE TABLE 表名
    ```

- 创建表

  - ```
    CREATE TABLE IF NOT EXISTS user(
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(50) COMMENT '姓名',
    age INT COMMENT '年龄',
    gender VARCHAR(1) COMMENT '性别'
    ) COMMENT '用户表';
    ```

- 查看创建表语句

  - ```
    SHOW CREATE TABLE 表名;
    ```



























