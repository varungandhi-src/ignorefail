```bash
❯ bazel build @com_github_linguist//:samples
ERROR: /private/var/tmp/_bazel_varun/e1174c7642f6b3887a41e855d468064b/external/com_github_linguist/BUILD.bazel:1:10: Label '@com_github_linguist//:samples/Starlark/filenames/BUILD' is invalid because '@com_github_linguist//samples/Starlark/filenames' is a subpackage; perhaps you meant to put the colon here: '@com_github_linguist//samples/Starlark/filenames:BUILD'?
ERROR: Skipping '@com_github_linguist//:samples': Error evaluating '@com_github_linguist//:samples': error loading package '@com_github_linguist//': Package '' contains errors
WARNING: Target pattern parsing failed.
ERROR: Error evaluating '@com_github_linguist//:samples': error loading package '@com_github_linguist//': Package '' contains errors
INFO: Elapsed time: 1.329s
INFO: 0 processes.
FAILED: Build did NOT complete successfully (1 packages loaded)
```

```bash
❯ bazel build @com_github_varun_linguist//:samples
INFO: Analyzed target @com_github_varun_linguist//:samples (2 packages loaded, 2891 targets configured).
INFO: Found 1 target...
Target @com_github_varun_linguist//:samples up-to-date (nothing to build)
INFO: Elapsed time: 1.248s, Critical Path: 0.00s
INFO: 1 process: 1 internal.
INFO: Build completed successfully, 1 total action
```
