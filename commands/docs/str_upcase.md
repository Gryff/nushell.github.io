---
title: str upcase
categories: |
  strings
version: 0.84.0
strings: |
  Make text uppercase.
usage: |
  Make text uppercase.
---

# <code>{{ $frontmatter.title }}</code> for strings

<div class='command-title'>{{ $frontmatter.strings }}</div>

## Signature

```> str upcase ...rest```

## Parameters

 -  `...rest`: For a data structure input, convert strings at the given cell paths


## Input/output types:

| input        | output       |
| ------------ | ------------ |
| list\<string\> | list\<string\> |
| record       | record       |
| string       | string       |
| table        | table        |
## Examples

Upcase contents
```shell
> 'nu' | str upcase
NU
```
