# PostgreSQL Cheat Sheet
PostgreSQL (psql) command lines in one page for the SQL REPL.

![YAP](https://i.imgur.com/flM2owb.gif)

## Basics
| Name | Description |
|------|-------------|
| `psql` | Connect to the database. |
| `psql -d pg_data_base -U pg_user` | Connect to localhost `pg_data_base` as `pg_user`. |
| `create user pg_user with password 'pguserpassword';` | Create a user `pg_user`. |
| `create database pg_database owner pg_user;` | Create a database with name `pg_database` which belongs to `pg_user`.


## General Purpose
| Name | Description |
|------|-------------|
| `\q` | Quit from psql. |
| `\l` | Lists all the databases. |
| `\dn` | List schemas. |
| `\dt` | List tables in connected database. |
| `\d table_name` | List columns on table. |
| `\df` | List functions |
| `\dv` | List views. |
| `\x auto` | Super pretty format query for long rows. |
| `\t` | Turn off/on output printing header and row count. |

Help me to fill out the rest useful commands which you think helpful to use on daily basis.
