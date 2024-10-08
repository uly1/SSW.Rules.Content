---
seoDescription: Schema guidelines recommend creating primary keys on tables to ensure data uniqueness and enable fast access.
type: rule
archivedreason:
title: Schema - Do you create primary key on your tables?
guid: c4682407-cea8-469a-abe4-8ddb795a986a
uri: create-primary-key-on-your-tables
created: 2019-11-05T23:57:23.0000000Z
authors:
  - title: Adam Cogan
    url: https://ssw.com.au/people/adam-cogan
related: []
redirects:
  - schema-do-you-create-primary-key-on-your-tables
---

When you specify a PRIMARY KEY constraint for a table, SQL Server enforces data uniqueness by creating a unique index for the primary key columns. This index also permits fast access to data when the primary key is used in queries.
Although, strictly speaking, the primary key is not essential - we recommend all tables have a primary key (except tables that have a high volume of continuous transactions).

::: bad
![Figure: Bad Example - Table missing primarykey](sql-table-without-primary-key.png)
:::

::: good
![Figure: Good Example - Table with primary key](sql-table-with-primary-key.png)
:::

**Legacy:**

Especially, when you have a client like Access, it would help you to avoid the problems.

<!--endintro-->
