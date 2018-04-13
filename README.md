# PostgreSQL Cheat Sheet
PostgreSQL (psql) commands in one page for the SQL REPL from [postgresql.org](https://www.postgresql.org/docs/10/static/index.html).

<img src="https://i.imgur.com/nueSCcH.gif" width="250">

## Basics
| Name | Description |
|------|-------------|
| `psql` | Connect to the database. |
| `psql -d <db> -U <user>` | Connect to localhost `db` as `user` name. |
| `psql create database <db>` | Create database with `db` name. |
| `create user <pg_user> with password '<password>';` | Create a user `pg_user` with `password`. |
| `create database <db> owner <user>;` | Create a database with name `db` which belongs to `user`.
| `create extension "uuid-ossp";` | Create useful extension with functions like `uuid_generate_v4`.
| `create extension "hstore";` | Create useful extension [hstore](https://www.postgresql.org/docs/current/static/hstore.html).
| `revoke all on database <db> from public;` |
| `grant connect on database <db> to <user>;` |
| `grant all on database <db> to <user>;` |


## General Purpose
| Name | Description |
|------|-------------|
| `\q` | Quit from psql. |
| `\?` | All commands of psql. |
| `\l+` | Lists all the databases with size. |
| `\c db_name` | Connect to database `db_name`. |
| `\dn` | List all schemas. |
| `\dt schema_name.*` | List all tables in `schema_name`. |
| `\d table_name` | List columns on table. |
| `\df` | List functions |
| `\dv` | List views. |
| `\x auto` | Super pretty query output for long rows. |
| `\t` | Turn off/on output header and row count. |
| `\h` | Help menu. |
| `\e` | Open an editor defined by your EDITOR environment variable, and put the most recent command entered in psql into the buffer. If it's vim editor use `shift + :` and tap `q` to quite or `wq` to resolve query. More vim [commands](https://vim.rtorr.com/). |
| `\ef [function]` | Open an editor, and put the function into the buffer. Without a function, it provides a convenient template for creating a new function. |
| `\s` | Print out your psql history to STDOUT. |
| `\timing` | Show timing for query execution. |


Hope you would be cool and efficient with this little cheat sheet.

Help me to fill out the rest useful commands which you think might be helpful to use on daily basis.
