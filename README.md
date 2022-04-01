`bazel build ...`:

```
INFO: Invocation ID: 50c6796a-5d9c-4363-82ab-f86237c0343e
DEBUG: /private/var/tmp/_bazel_johnfirebaugh/9875e3601c9a8dfff06a3f45aaaf7414/external/build_bazel_rules_nodejs/index.bzl:65:14: node_repository attribute not set and no repository named 'nodejs_toolchains' exists; installing default node
INFO: Analyzed 4 targets (0 packages loaded, 0 targets configured).
INFO: Found 4 targets...
ERROR: /Users/john/figma/scratch/fullscreen/node-fields-codegen/BUILD.bazel:3:11: Compiling TypeScript project //fullscreen/node-fields-codegen:ts [tsc -p fullscreen/node-fields-codegen/tsconfig.json] failed: (Exit 2): tsc.sh failed: error executing command bazel-out/darwin-opt-exec-2B5CBBC6/bin/external/npm/typescript/bin/tsc.sh --project fullscreen/node-fields-codegen/tsconfig.json --outDir bazel-out/darwin-fastbuild/bin/fullscreen/node-fields-codegen ... (remaining 3 arguments skipped)

Use --sandbox_debug to see verbose messages from the sandbox
[snip traceResolution output]
fullscreen/node-fields-codegen/src/api-codegen.ts(1,23): error TS2307: Cannot find module '../../../share/kiwi/js/kiwi' or its corresponding type declarations.
INFO: Elapsed time: 0.894s, Critical Path: 0.73s
INFO: 2 processes: 2 internal.
FAILED: Build did NOT complete successfully
```
