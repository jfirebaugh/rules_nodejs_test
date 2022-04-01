`bazel build ...`:

```
INFO: Invocation ID: a775f31d-29fc-4650-a74b-eed112f5c01c
DEBUG: /private/var/tmp/_bazel_johnfirebaugh/9875e3601c9a8dfff06a3f45aaaf7414/external/build_bazel_rules_nodejs/index.bzl:65:14: node_repository attribute not set and no repository named 'nodejs_toolchains' exists; installing default node
INFO: Analyzed 4 targets (0 packages loaded, 0 targets configured).
INFO: Found 4 targets...
ERROR: /Users/john/figma/scratch/a/BUILD.bazel:3:11: Compiling TypeScript project //a:ts [tsc -p a/tsconfig.json] failed: (Exit 2): tsc.sh failed: error executing command bazel-out/darwin-opt-exec-2B5CBBC6/bin/external/npm/typescript/bin/tsc.sh --project a/tsconfig.json --outDir bazel-out/darwin-fastbuild/bin/a --rootDir a ... (remaining 1 argument skipped)

Use --sandbox_debug to see verbose messages from the sandbox
a/a.ts(1,19): error TS2307: Cannot find module '../b/b' or its corresponding type declarations.
INFO: Elapsed time: 0.907s, Critical Path: 0.74s
INFO: 2 processes: 2 internal.
FAILED: Build did NOT complete successfully
```
