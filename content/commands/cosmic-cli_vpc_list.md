---
date: 2019-07-22T15:05:55+02:00
title: "cosmic-cli vpc list"
---
List VPCs

```text
cosmic-cli vpc list [flags]
```

## Options

```text
  -f, --filter strings          filter results (supports regex)
  -h, --help                    help for list
  -p, --profile string          specify profile(s) to use
      --reverse-sort            reverse sort order
      --show-id                 show VPC id in result
      --show-redundant-status   show VPC redundant router status in result
      --show-restart-required   show VPC restart required status in result
      --show-snat               show VPC Source NAT IP in result
  -s, --sort-by string          field to sort by (default "name")
```

## SEE ALSO

* [cosmic-cli vpc](../cosmic-cli_vpc/) - VPC subcommands
