package(default_visibility = ["//visibility:public"])

filegroup(
    name = "dart_vm_binary",
    srcs = select({
        "//dart:darwin": ["dart_vm_binary.sh"],
        "//dart:k8": ["dart_vm_binary.sh"],
        "//dart:windows": ["dart_vm_binary.cmd"],
    }),
)

filegroup(
    name = "dart_vm_test_template",
    srcs = select({
        "//dart:coverage_config": [":dart_vm_test_coverage"],
        "//conditions:default": [":dart_vm_test"],
    }),
)

filegroup(
    name = "dart_vm_test",
    srcs = select({
        "//dart:darwin": ["dart_vm_test.sh"],
        "//dart:k8": ["dart_vm_test.sh"],
        "//dart:windows": ["dart_vm_test.cmd"],
    }),
)

filegroup(
    name = "dart_vm_test_coverage",
    srcs = select({
        "//dart:darwin": ["dart_vm_test_coverage.sh"],
        "//dart:k8": ["dart_vm_test_coverage.sh"],
        "//dart:windows": ["dart_vm_test_coverage.cmd"],
    }),
)
