---
title: "Setup"
weight: 15
date: 2019-07-21T11:28:51+02:00
draft: true
---

Cosmic CLI requires a config file at `$HOME/.cosmic-cli/config.toml` to run. This file should contain each Cosmic API you want to run commands against.

Below is an example config file:

```text
[profiles.zone1]
api_url    = "https://zone1/client/api"
api_key    = "<zone1 api key>"
secret_key = "<zone1 secret key>"

[profiles.zone2]
api_url    = "https://zone2/client/api"
api_key    = "<zone2 api key>"
secret_key = "<zone2 secret key>"

[profiles.zone3]
api_url    = "https://zone3/client/api"
api_key    = "<zone3 api key>"
secret_key = "<zone3 secret key>"
```

By default the CLI commands are ran against all configured profiles.  If you want to select which profiles to use you can use the `-p` option.

For example, to run a command against a single profile:

```
cosmic-cli vpc list -p zone1
```

or to run against multiple profiles:

```
cosmic-cli vpc list -p zone1,zone2
```
