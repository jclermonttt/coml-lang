# COML

Coml's Obvious, Minimal Language.

By Jeremy Clermont.

## Objectives

## Table of contents

## Preliminaries

## Comment

```coml
#! This is a full-line comment
key = "value" #! This is a comment at the end of a line
another = "#! This not a commment"

#!
* This is a multiple-line
* comment example...
!#
{example}
key = "value"
```

Comments should be used to communicate between the human readers of a file.

## Key/Value Pair

The primary building block of a COML document is the key/value pair.

Keys are on the left of the equals sign and values are on the right.
Whitespace is ignored around key names and values. The key, equals sign, and values must be on the same line ().

```coml
key = "value"
```

Values must have one of the following types.

- [String]()
- [Integer]()
- [Float]()
- [Boolean]()
- [Offset Date-Time]()
- [Local Date-Time]()
- [Local Date]()
- [Local Time]()
- [Array]()
- [Inline Table]()

Unspecified values are invalid.

```coml
key = #! INVALID
```

There must be a newline after a key/value pair.

```coml
first = "Jeremy" last = "Clermont" #! INVALID
```

## Keys

Keys are case-sensitive and should be alphanumeric, allowing hyphens `-` but not underscores `_`.

```coml
key = "value"
1234 = "value"
bare-key = "value"
bare_key = "value" #! INVALID
```
**Dotted keys**

```coml
name = "Orange"
physical.color = "orange"

```

In JSON land, that would give you the following structure: 

```json
{
    "name": "Orange",
    
}
```

## String

## Float

## Boolean

## Offset Date-Time

## Local Date-Time

## Local Date

## Array

## Table

## Inline Table

## Curly Braces of Tables

## Filename Extension

COML files should use the extension `.coml`.
