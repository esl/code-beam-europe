---
tags:	
- Data processing and transformation
level: Intermediate
title: 	"Building Analytic Systems with Elixir"
speakers:
- _participants/dmitry-russ.md

---
This is a case study and discussion about state of the art for developing analytical systems with Elixir. Multiple years we are working on Process Mining products with Elixir, using and experimenting with different technologies (Clickhouse, MariaDB column storage, DuckDB, KDB+, Polars). This talk is about problems, design decisions and challenges on the way, like developing in-house ecto-like framework, explaining what you can't achieve with SQL and why you might look into lower-level technology like Polars & KDB+, ending with trying to show-case some example functionalities on top of Elixir Explorer and comparing them with Python.