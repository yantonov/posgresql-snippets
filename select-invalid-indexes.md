Select invalid indexes

```sql
SELECT ns.nspname, clz.relname,*
FROM
       pg_class as clz

       JOIN
       pg_index as idx
       ON clz.oid=idx.indexrelid

       JOIN pg_namespace as ns
       ON clz.relnamespace=ns.oid

WHERE
        idx.indisvalid = false
ORDER BY ns.oid;
```
References:  
1. [pg_class](https://www.postgresql.org/docs/current/static/catalog-pg-class.html)
2. [pg_index](https://www.postgresql.org/docs/current/static/catalog-pg-index.html)
3. [pg_namespace](https://www.postgresql.org/docs/current/static/index.html)
