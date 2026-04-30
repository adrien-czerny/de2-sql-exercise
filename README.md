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

This is a vague ask on purpose; the business likes to keep things fuzzy. Feel
free to ask for clarifications and we'll provide guidance. We are more
interested in your workings than to get to a "final" result.

To get you started, here are a few leads:
* Poke at the data! In particular, `swapi_people`, `swapi_films` & `swapi_species`
* Can you see anything that jumps out as relevant to the concept of inclusivity?
* Think about the grain of the data; in your ideal resulting dataset, what would be a "unique" key?

Even if it's not necessary to fulfil the ask, we may ask you to go over:
* Handling of discrepancies
* Joining of tables
* Organising SQL as CTEs

## Setup

A DuckDB database file is provided to you in this repo. To install DuckDB you
can follow along at:
https://duckdb.org/install/?platform=linux&environment=cli. You can then run
the local DuckDB UI and connect to the database file in a terminal:

```
$ duckdb -ui ./wh.db
```

Alternatively, with docker:

```
$ docker run --rm -it -v "$(pwd):/workspace" -w /workspace --net host duckdb/duckdb duckdb -ui wh.db
```
