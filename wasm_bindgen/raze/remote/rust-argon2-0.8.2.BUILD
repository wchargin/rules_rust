"""
@generated
cargo-raze crate build file.

DO NOT EDIT! Replaced on runs of cargo-raze
"""

# buildifier: disable=load
load(
    "@io_bazel_rules_rust//rust:rust.bzl",
    "rust_binary",
    "rust_library",
    "rust_test",
)

# buildifier: disable=load
load("@bazel_skylib//lib:selects.bzl", "selects")

package(default_visibility = [
    # Public for visibility by "@raze__crate__version//" targets.
    #
    # Prefer access through "//wasm_bindgen/raze", which limits external
    # visibility to explicit Cargo.toml dependencies.
    "//visibility:public",
])

licenses([
    "notice",  # MIT from expression "MIT OR Apache-2.0"
])

# Generated targets

alias(
    name = "rust_argon2",
    actual = ":argon2",
    tags = [
        "cargo-raze",
        "manual",
    ],
)

# buildifier: leave-alone
rust_library(
    name = "argon2",
    crate_type = "lib",
    deps = [
        "@rules_rust_wasm_bindgen__base64__0_12_3//:base64",
        "@rules_rust_wasm_bindgen__blake2b_simd__0_5_10//:blake2b_simd",
        "@rules_rust_wasm_bindgen__constant_time_eq__0_1_5//:constant_time_eq",
        "@rules_rust_wasm_bindgen__crossbeam_utils__0_7_2//:crossbeam_utils",
    ],
    srcs = glob(["**/*.rs"]),
    crate_root = "src/lib.rs",
    edition = "2018",
    rustc_flags = [
        "--cap-lints=allow",
    ],
    version = "0.8.2",
    tags = [
        "cargo-raze",
        "manual",
    ],
    crate_features = [
        "crossbeam-utils",
        "default",
    ],
)
# Unsupported target "integration_test" with type "test" omitted
