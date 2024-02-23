# Bazel rules_go SDK version update issue reproducer

This is a test repo used to reproduce the https://github.com/bazelbuild/rules_go/issues/3436 issue.

I tried the do what @fmeum suggested in https://github.com/bazelbuild/rules_go/issues/3436#issuecomment-1410410673
and it seems to work just fine:

```console
$ bazel run //:sdkversionrepro                         
Go version: go1.22.0 X:nocoverageredesign
```

It's not clear if https://github.com/bazelbuild/rules_go/issues/3436 or if I'm misunderstanding the issue.
