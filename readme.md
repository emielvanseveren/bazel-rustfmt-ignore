Steps to reproduce:

1. Install bazelisk or bazel with version mentioned in `.bazelversion` file. 
1. Run `CARGO_BAZEL_REPIN=1 bazel sync --only=crate_index`
2. Run `bazel run @rules_rust//:rustfmt  --@rules_rust//:rustfmt.toml=//:rustfmt.toml --output_groups=+rustfmt_checks`
