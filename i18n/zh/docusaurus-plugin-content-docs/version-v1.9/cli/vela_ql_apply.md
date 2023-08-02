---
title: vela ql apply
---

Create and store a VelaQL view

### Synopsis

Create and store a VelaQL view to reuse it later.

You can specify your view file from:
	- a file (-f my-view.cue)
	- a URL (-f https://example.com/view.cue)
	- stdin (-f -)

View name can be automatically inferred from file/URL.
If we cannot infer a name from it, you must explicitly specify the view name (see examples).

If a view with the same name already exists, it will be updated.

```
vela ql apply [view-name] [flags]
```

### Examples

```
Assume your VelaQL view is stored in <my-view.cue>.

View name will be implicitly inferred from file name or URL (my-view):
	vela ql create -f my-view.cue

You can also explicitly specify view name (custom-name):
	vela ql create custom-name -f my-view.cue

If view name cannot be inferred, or you are reading from stdin (-f -), you must explicitly specify view name:
	cat my-view.cue | vela ql create custom-name -f -
```

### Options

```
  -f, --file string   CUE file that stores the view, can be local path, URL, or stdin (-)
  -h, --help          help for apply
```

### Options inherited from parent commands

```
  -V, --verbosity Level   number for the log level verbosity
  -y, --yes               Assume yes for all user prompts
```

### SEE ALSO

* [vela ql](vela_ql)	 - Show result of executing velaQL.

#### Go Back to [CLI Commands](vela) Homepage.


###### Auto generated by [spf13/cobra script in KubeVela](https://github.com/kubevela/kubevela/tree/master/hack/docgen).