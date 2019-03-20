Select full text search configuration

```psql
\dF
```

```sql
select oid, * from pg_catalog.pg_ts_config;
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
3. [pg-ts-config-map](https://www.postgresql.org/docs/current/catalog-pg-ts-config-map.html)
4. [pg-ts-dict](https://www.postgresql.org/docs/current/catalog-pg-ts-dict.html)
5. [pg-ts-parser](https://www.postgresql.org/docs/current/catalog-pg-ts-parser.html)
6. [pg-ts-template](https://www.postgresql.org/docs/current/catalog-pg-ts-template.html)
7. [ts_token_type](https://www.postgresql.org/docs/current/textsearch-debugging.html)
8. [textsearch-psql](https://www.postgresql.org/docs/current/textsearch-psql.html)
