# Data Pipeline
A data pipeline is a set of actions that ingest raw data from disparate sources and move the data to a destination for storage and analysis. A pipeline also may include filtering and features that provide resiliency against failure.


##  SELECT


### Show current user 

```sql
select user from dual;
```

### Calculate rows in a table named Stars
```sql
select count(*) from Stars;
```

### Calculate aggregrate function from Stars table on Age Column
```sql
select MIN(Age), MAX(Age), AVG(Age) from Stars group by Age;
```

## Sample duplicate values in a column
```sql
SELECT column_name, COUNT(*)
FROM test_table
GROUP BY column_name
HAVING COUNT(*) > 1;
```

