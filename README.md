# golang-postgres
## Basic postgres commands
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
```

### File Structure
- middleware
    - handler.go `(server logic)`

- models
    - stocks.go `(sql model for table)`

- router
    - router.go `(controller for routing http)`

- main.go