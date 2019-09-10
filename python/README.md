Attempt to understand Ethereum's data model using [ether_sql](https://github.com/analyseether/ether_sql) for ER diagram to help visually understand.

```
go get -u github.com/achiku/planter
brew install plantuml

docker-compose up -d
docker-compose run --rm python ether_sql sql upgrade_tables
planter "postgres://finney:password@localhost/ether_sql?sslmode=disable" -o ether_sql.uml
plantuml ether_sql.uml
open ether_sql.png
```

- https://github.com/analyseether/ether_sql
- https://github.com/achiku/planter
