# Intergalactic pair programming brief

We'll be your copilot(s) during this pair programming exercise, and we'll be
looking at your thought process, research skills and Python proficiency.

BE OVERLY VERBOSE/TALKATIVE. Run yourself with `--verbose` e.g. ask questions
or explain your rationale. That'll give us better insights into your
capabilities, and let us hand you gists/code snippets we've got at the ready so
you don't have to do too much research.

## Context

The business has ingested a lot of Star Wars data in its Data Warehouse as a
DuckDB database. It now has great needs for insights, and all the BI Analysts
are on holiday.

## Ask

Run some SQL to give the important insights to the Business:

> How inclusive are Star Wars movies? Show movie title and release years.

## Instructions

A DuckDB database file is provided to you in this repo. You can run the local
DuckDB UI and connect to the database file in a terminal:

```
$ duckdb -ui ./wh.db
```

Alternatively, with docker:

```
$ docker run --rm -it -v "$(pwd):/workspace" -w /workspace --net host duckdb/duckdb duckdb -ui wh.db
```
