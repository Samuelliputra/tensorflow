licenses(["restricted"])

package(default_visibility = ["//visibility:public"])

# Platform for use with remote execution with
# custom container based off RBE Ubuntu16_04
# http://gcr.io/cloud-marketplace/google/rbe-ubuntu16-04
# Built with //tensorflow/tools/ci_build/Dockerfile.rbe.cpu
platform(
    name = "rbe_ubuntu16_04-tf",
    constraint_values = [
        "@bazel_tools//platforms:x86_64",
        "@bazel_tools//platforms:linux",
        "@bazel_tools//tools/cpp:clang",
        "@bazel_toolchains//constraints:xenial",
    ],
    remote_execution_properties = """
        properties: {
            name: "container-image"
            value:"docker://gcr.io/asci-toolchain/nosla-ubuntu16_04-tf@sha256:495a025ed5e273cfa5d53357ef93ac20500c008994e0be106c509f51555fb93c"
        }""",
)

platform(
    name = "rbe_cuda9.0-cudnn7-ubuntu14.04",
    constraint_values = [
        "@bazel_tools//platforms:x86_64",
        "@bazel_tools//platforms:linux",
        "@bazel_tools//tools/cpp:clang",
        "@bazel_toolchains//constraints:xenial",
    ],
    remote_execution_properties = """
        properties: {
            name: "container-image"
            value:"docker://gcr.io/asci-toolchain/nosla-cuda9.0-cudnn7-ubuntu14.04@sha256:06b585f42eed3b2030e9566b8f88f48d7472fa0f47e59765bc115376c8801bdf"
        }""",
)
