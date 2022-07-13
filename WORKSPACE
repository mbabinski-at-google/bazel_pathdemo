workspace(name = "bazel_pathdemo")

load('@bazel_tools//tools/build_defs/repo:git.bzl', 'git_repository')

git_repository(
    name = "com_google_protobuf",
    commit = '6556fb3aba6737136982e096e21b97a95493171e',
    remote = 'https://github.com/protocolbuffers/protobuf.git'
)

load("@com_google_protobuf//:protobuf_deps.bzl", "protobuf_deps")
protobuf_deps()
