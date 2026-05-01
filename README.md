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

## Setup

A DuckDB database file is provided to you in this repo. To install DuckDB you
can follow along at: https://duckdb.org/install/. You can then run the local
DuckDB UI and connect to the database file in a terminal:

```
$ duckdb -ui ./wh.db
```

**Not supported specifically on Windows machines with an ARM64 architecture**.

Alternatively, try with docker:

```
$ docker run --rm -it -v "$(pwd):/workspace" -w /workspace --net host duckdb/duckdb duckdb -ui wh.db
```

## Ask

Answer one or more from the following questions:
* Show each character name along with the vehicle name this character is driving the most (Easy)
* Show a count of each gender that each movie includes; show the movie name, order by release date (Med)
* Show the most prolific pair of characters i.e. order each pair of character depending on how often they appear together in a movie (Hard)

Hints:
* Keep an eye out for discrepancies and missing values!
* Think of organising your SQL in CTEs
