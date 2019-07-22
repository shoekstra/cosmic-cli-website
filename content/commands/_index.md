---
title: "Commands"
weight: 20
date: 2019-07-21T11:28:02+02:00
---

On the left is a command reference of all Cosmic CLI commands and their sub-commands.

## Command help

Help for a specific subcommand is available by running `cosmic-cli help <subcommand>` or `cosmic-cli <subcommand> -h`.

## Filtering results

Cosmic CLI commands are ran against all configured profiles, meaning sometimes you'll get many results when you're just looking for one or a few.

To filter a result use `-f field=value`, where `field` can be any table header and `value` is parsed as a regex for more flexible filtering. Sometimes you may need to use a `--show` command to show additional fields for filtering.

To filter results where the name field contains "vdi":

```text
-f name=vdi
```

When filtering for a value with spaces, put the filter in quotes:

```text
-f 'name=vdi 2'
```

You can use multiple filters by calling `-f` multiple times:

```text
-f name=vdi -f vpcofferingname=default
```

Or you can pass a list to `-f`:

```text
-f name=vdi,vpcofferingname=default
```
