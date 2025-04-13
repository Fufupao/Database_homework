### 题目一
> 1. 新建一个`university`数据库，并执行`largeRelationsInsertFile.sql`，导入数据。
> 2. 运行第2次作业的题目三代码。注意：把原题目中的`会计`改成`History`。  

1.
- 新建一个`university`数据库。

![](https://github.com/Fufupao/Database_SQL/blob/main/image/work3/3.1.1.png?raw=true)

- 执行`largeRelationsInsertFile.sql`，导入数据。

![](https://github.com/Fufupao/Database_SQL/blob/main/image/work3/3.1.2.png?raw=true)

2.
- 运行第2次作业的题目三代码。

![](https://github.com/Fufupao/Database_SQL/blob/main/image/work3/3.1.3.png?raw=true)  

![](https://github.com/Fufupao/Database_SQL/blob/main/image/work3/3.1.4.png?raw=true)

结果为空，没有找到符合要求的数据。

### 题目二
>参考[Pattern Matching](https://www.postgresql.org/docs/17/functions-matching.html)，在PG中使用至少三种方法实现找到所有以`S`开头教师的名字。

```sql
-- 方法1 ~ LIKE  
SELECT name  
FROM instructor  
WHERE name LIKE 'S%';  

-- 方法2 ~ SIMILAR TO Regular Expressions  
SELECT name  
FROM instructor  
where name SIMILAR TO 'S%';  

-- 方法3 ~ POSIX Regular Expressions  
SELECT name  
FROM instructor  
where name ~ 'S.*';
```

运行结果均为：

![](https://github.com/Fufupao/Database_SQL/blob/main/image/work3/3.2.1.png?raw=true)

### 题目三
> `psql`是PostgreSQL的命令行工具。请使用`psql`命令行工具：
> 
> - 实现题目二
> - 列出所有的数据库
> - 列出当前数据库的所有表
> - 显示某张表的关系模式


- 实现题目二

![](https://github.com/Fufupao/Database_SQL/blob/main/image/work3/3.3.1.png?raw=true)

- 列出所有的数据库

![](https://github.com/Fufupao/Database_SQL/blob/main/image/work3/3.3.2.png?raw=true)

- 列出当前数据库的所有表

![](https://github.com/Fufupao/Database_SQL/blob/main/image/work3/3.3.3.png?raw=true)

- 显示某张表的关系模式

![](https://github.com/Fufupao/Database_SQL/blob/main/image/work3/3.3.4.png?raw=true)

