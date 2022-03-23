# Pre-commit config file for SQL scripts

## Folders structure 

* generic - customized SQL fluff config for generic unsupported SQL dialect
* mysql - customized SQL fluff config for MySQL dialect

## Installation

Install [pre-commit](https://pre-commit.com/) and [sqlfluff](https://www.sqlfluff.com/)

```console
$ python -m pip install sqlfluff 
$ python -m pip install pre-commit
```
Update all hooks in config file:

```console
$ python -m pre-commit autoupdate
```

## Operation

1. Copy required config file from generic or mysql folder to SQL project folder

2. Run git hooks with pre-commit

For manual run (before every commit):

```console
$ python -m pre-commit run
```

For auto run (once for project):

```console
$ python -m pre-commit install
```