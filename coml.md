

## Comment

```coml
#! This is a full-line comment
key = "value"
another = { "#! This is not a comment" }
```


## Table

Tables are collections of key/value
pairs.

```coml
{table}
```

## Variable and Reference

```coml
{database}
host = "localhost"
port = 5432

{development}
db-host = ${database.host}
db-port = ${database.port}
```

## Imports

```coml
{include}
path = "config/common.coml"
```

## Curly Brace of Tables

```coml
{services}
{{web}}
name = "Web Server"
port = 80
enabled = true

{{web}}
name = "API Server"
port = 8080
enabled = true

{{database}}
name = "Primary Database"
ip = "192.168.1.10"
port = 5432
enabled = true

{{database}}
name = "Secondary Database"
ip = "192.168.1.11"
port = 5432
enabled = false
```