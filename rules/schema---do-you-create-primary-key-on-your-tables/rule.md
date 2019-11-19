---
type: rule
archivedreason: 
title: Schema - Do you create primary key on your tables?
guid: c4682407-cea8-469a-abe4-8ddb795a986a
uri: schema---do-you-create-primary-key-on-your-tables
created: 2019-11-05T23:57:23.0000000Z
authors:
- id: 1
  title: Adam Cogan
related: []

---

When you specify a PRIMARY KEY constraint for a table, SQL Server enforces data uniqueness by creating a unique index for the primary key columns. This index also permits fast access to data when the primary key is used in queries.
Although, strictly speaking, the primary key is not essential - we recommend all tables have a primary key (except tables that have a high volume of continuous transactions).
<dl class="ssw15-rteElement-ImageArea"><img src="SqlTableWithoutPrimaryKey.PNG" alt="" style="margin:5px;"></dl>

::: bad
Figure: Bad Example - Table missing primarykey

:::

<dl class="ssw15-rteElement-ImageArea"><img src="SqlTableWithPrimaryKey.PNG" alt="" style="margin:5px;"></dl>

::: good
Figure: Good Example - Table with primary key

:::

<dl class="ssw15-rteElement-ImageArea"><br></dl>
**Legacy:**

Especially, when you have a client like Access, it would help you to avoid the problems.

<!--endintro-->