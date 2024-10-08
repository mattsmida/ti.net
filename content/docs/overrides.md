---
lang: en
title: 'Timewarrior - Overrides'
viewport: 'width=device-width, initial-scale=1'
hide_toc: true
---

# Overrides

Using the override syntax, you can temporarily modify configuration settings from the command line, for one command only.
The syntax is:

```console
rc.<name>[=<value>]
```

Timewarrior operates in verbose mode by default:

```console
$ timew start
Tracking
  Started 2016-06-19T09:18:38
  Current                  38
  Total               0:00:00
```

This can be temporarily disabled using the override like this:

```console
$ timew start rc.verbose=off
```

Without verbose mode, no feedback is generated.
Another way to do this is to use the `:quiet` hint, which does the same thing, but only a few settings have corresponding hints:

```console
$ timew start :quiet
```

To make this a permanent choice, use the `config` command:

```console
$ timew config verbose off
...
```
