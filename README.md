# golang-postgres

## Connect with SQL using the default `database/sql` module
The advantage of this type is, the user can write the required SQL queries instead of depending on ORM APIs

### Basic postgres commands
Start postgres server
```
sudo service postgresql start
```
Access postgres-cli
```
psql -U postgres
```
Create Database
```
CREATE DATABASE <DB_NAME>;
```
Connect to the Database
```
\c <DB_NAME>;
```
Create Table
```
CREATE TABLE <TABLE_NAME> (<ATTR_NAME> <ATTR_TYPE>, ...);
```
### Required dependencies
```
github.com/gorilla/mux
github.com/joho/godotenv
github.com/lib/pq (To point to the sql driver)
```

### File Structure
- middleware
    - handler.go `(server logic)`

- models
    - stocks.go `(sql model for table)`

- router
    - router.go `(controller for routing http)`

- main.go