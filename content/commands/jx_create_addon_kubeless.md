---
date: 2019-05-11T08:10:08Z
title: "jx create addon kubeless"
slug: jx_create_addon_kubeless
url: /commands/jx_create_addon_kubeless/
---
## jx create addon kubeless

Create a kubeless addon for hosting Git repositories

### Synopsis

Creates the kubeless addon for serverless on Kubernetes

```
jx create addon kubeless [flags]
```

### Examples

```
  # Create the kubeless addon in the kubeless namespace
  jx create addon kubeless
  
  # Create the kubeless addon in a custom namespace
  jx create addon kubeless -n mynamespace
```

### Options

```
  -c, --chart string         The name of the chart to use (default "incubator/kubeless")
      --helm-update          Should we run helm update first to ensure we use the latest version (default true)
  -h, --help                 help for kubeless
  -n, --namespace string     The Namespace to install into (default "kubeless")
  -r, --release string       The chart release name (default "kubeless")
  -s, --set string           The chart set values (can specify multiple or separate values with commas: key1=val1,key2=val2)
  -f, --values stringArray   List of locations for values files, can be local files or URLs
  -v, --version string       The chart version to install)
```

### Options inherited from parent commands

```
  -b, --batch-mode                Runs in batch mode without prompting for user input (default true)
      --install-dependencies      Enables automatic dependencies installation when required
      --log-level string          Sets the logging level (panic, fatal, error, warning, info, debug) (default "info")
      --no-brew                   Disables brew package manager on MacOS when installing binary dependencies
      --skip-auth-secrets-merge   Skips merging the secrets from local files with the secrets from Kubernetes cluster
      --verbose                   Enables verbose output
```

### SEE ALSO

* [jx create addon](/commands/jx_create_addon/)	 - Creates an addon

###### Auto generated by spf13/cobra on 11-May-2019