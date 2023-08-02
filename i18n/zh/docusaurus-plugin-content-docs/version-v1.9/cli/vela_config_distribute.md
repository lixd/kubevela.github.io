---
title: vela config distribute
---

Distribute a config

```
vela config distribute [flags]
```

### Examples

```
  # distribute the config(test-registry) from the vela-system namespace to the default namespace in the local cluster.
  vela config d test-registry -t default
  
  # distribute the config(test-registry) from the vela-system namespace to the other clusters.
  vela config d test-registry -t cluster1/default -t cluster2/default
  
  # recall the config
  vela config d test-registry --recall
```

### Options

```
  -h, --help                 help for distribute
  -n, --namespace string     specify the namespace of the distribution (default "vela-system")
  -r, --recall               this field means recalling the configs from all targets.
  -t, --target stringArray   specify the targets that want to distribute,the format is: <clusterName>/<namespace>
```

### Options inherited from parent commands

```
  -V, --verbosity Level   number for the log level verbosity
  -y, --yes               Assume yes for all user prompts
```

### SEE ALSO

* [vela config](vela_config)	 - Manage the configs.

#### Go Back to [CLI Commands](vela) Homepage.


###### Auto generated by [spf13/cobra script in KubeVela](https://github.com/kubevela/kubevela/tree/master/hack/docgen).