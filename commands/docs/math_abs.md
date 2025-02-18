---
title: math abs
categories: |
  math
version: 0.84.0
math: |
  Returns the absolute value of a number.
usage: |
  Returns the absolute value of a number.
---

# <code>{{ $frontmatter.title }}</code> for math

<div class='command-title'>{{ $frontmatter.math }}</div>

## Signature

```> math abs ```


## Input/output types:

| input          | output         |
| -------------- | -------------- |
| duration       | duration       |
| list\<duration\> | list\<duration\> |
| list\<number\>   | list\<number\>   |
| number         | number         |
## Examples

Compute absolute value of each number in a list of numbers
```shell
> [-50 -100.0 25] | math abs
╭───┬────────╮
│ 0 │     50 │
│ 1 │ 100.00 │
│ 2 │     25 │
╰───┴────────╯

```
