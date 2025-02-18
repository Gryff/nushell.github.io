---
title: dfr value-counts
categories: |
  dataframe
version: 0.84.0
dataframe: |
  Returns a dataframe with the counts for unique values in series.
usage: |
  Returns a dataframe with the counts for unique values in series.
---

# <code>{{ $frontmatter.title }}</code> for dataframe

<div class='command-title'>{{ $frontmatter.dataframe }}</div>

## Signature

```> dfr value-counts ```


## Input/output types:

| input | output |
| ----- | ------ |
| any   | any    |

## Examples

Calculates value counts
```shell
> [5 5 5 5 6 6] | dfr into-df | dfr value-counts
╭───┬───┬────────╮
│ # │ 0 │ counts │
├───┼───┼────────┤
│ 0 │ 5 │      4 │
│ 1 │ 6 │      2 │
╰───┴───┴────────╯

```


**Tips:** Dataframe commands were not shipped in the official binaries by default, you have to build it with `--features=dataframe` flag