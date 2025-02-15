
# COML

Clarus Obvious, Minimal Language.

By Jeremy Clermont.

## Example

```coml
#! This is a COML document.

title = "COML EXAMPLE"

{owner}
name = "Jeremy Clermont"

{database}
server = "192.168.1.1"
ports = { 8000, 8001, 8002 }
connection-max = 6000
enabled = true

{clients}
data = { ["gamma", "delta"], ["1", "2"] }

#! Line breaks are OK when inside curly braces
hosts = {
    "alpha",
    "omega"
}

```


## Filename Extension

COML files should use the extension `.coml`,