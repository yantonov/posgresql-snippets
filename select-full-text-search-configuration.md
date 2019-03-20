Select full text search configuration

```psql
\dF
```

```sql
select * from pg_catalog.pg_ts_config;
```

Select full text search dictionaries

```psql
\dFd
```

```sql
SELECT dictname FROM pg_catalog.pg_ts_dict;
```

References:  
1. [full text search](https://www.postgresql.org/docs/current/textsearch.html)
2. [pg_ts_config](https://www.postgresql.org/docs/current/catalog-pg-ts-config.html)
3. [catalog-pg-ts-dict](https://www.postgresql.org/docs/current/catalog-pg-ts-dict.html)
4. [textsearch-psql](https://www.postgresql.org/docs/current/textsearch-psql.html)
