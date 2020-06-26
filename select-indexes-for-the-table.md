Select all indexes for the table

```sql
SELECT i.relname as indexname, t.relname as tablename, t.OID
FROM pg_class i
JOIN pg_index idx ON idx.indexrelid = i.oid
JOIN pg_class t ON t.oid = idx.indrelid
WHERE i.relkind = 'I'
ORDER BY tablename;
```

References:  
1. [pg_class](https://www.postgresql.org/docs/current/static/catalog-pg-class.html)
2. [pg_index](https://www.postgresql.org/docs/current/static/catalog-pg-index.html)
