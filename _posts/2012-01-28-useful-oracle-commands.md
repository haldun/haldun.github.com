---
layout: post
title: Useful Oracle Queries
---

{{ page.title }}
================

### Getting current schema

```
select sys_context('userenv', 'current_schema') from dual;
```

### Changing current schema

```
alter session set current_schema = new_schema;
```

### Listing tables

```
select table_name from user_tables;
````

### Dropping all tables

```
select 'drop table '||table_name||' cascade constraints;' from user_tables;
```

Note that, the query above will generate delete query for each table. You should execute those generated queries to actually delete the tables.

### Modifying a field

```
alter table EPISODES modify(bitrate null);
```
