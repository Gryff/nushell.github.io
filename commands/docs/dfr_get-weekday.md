---
title: dfr get-weekday
categories: |
  dataframe
version: 0.84.0
dataframe: |
  Gets weekday from date.
usage: |
  Gets weekday from date.
---

# <code>{{ $frontmatter.title }}</code> for dataframe

<div class='command-title'>{{ $frontmatter.dataframe }}</div>

## Signature

```> dfr get-weekday ```


## Input/output types:

| input | output |
| ----- | ------ |
| any   | any    |

## Examples

Returns weekday from a date
```shell
> let dt = ('2020-08-04T16:39:18+00:00' | into datetime -z 'UTC');
    let df = ([$dt $dt] | dfr into-df);
    $df | dfr get-weekday
╭───┬───╮
│ # │ 0 │
├───┼───┤
│ 0 │ 2 │
│ 1 │ 2 │
╰───┴───╯

```


**Tips:** Dataframe commands were not shipped in the official binaries by default, you have to build it with `--features=dataframe` flag