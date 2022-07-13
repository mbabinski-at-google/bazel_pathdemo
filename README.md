```
maciej@euler:~/src/bazel_pathdemo$ blaze build @com_google_protobuf//:protobuf_python
ERROR: /home/maciej/.cache/bazel/_bazel_maciej/9b06658a951c05e81a0ba5e98fa64f19/external/com_google_protobuf/python/BUILD.bazel:52:20: in internal_copy_files_impl rule @com_google_protobuf//python:copied_wkt_proto_files:
Traceback (most recent call last):
        File "/home/maciej/.cache/bazel/_bazel_maciej/9b06658a951c05e81a0ba5e98fa64f19/external/com_google_protobuf/python/internal.bzl", line 11, column 17, in _internal_copy_files_impl
                fail("Source does not start with %s: %s" %
Error in fail: Source does not start with src/: ../com_google_protobuf/src/google/protobuf/descriptor.proto
ERROR: /home/maciej/.cache/bazel/_bazel_maciej/9b06658a951c05e81a0ba5e98fa64f19/external/com_google_protobuf/python/BUILD.bazel:52:20: Analysis of target '@com_google_protobuf//python:copied_wkt_proto_files' failed
ERROR: Analysis of target '@com_google_protobuf//:protobuf_python' failed; build aborted:
INFO: Elapsed time: 0.676s
INFO: 0 processes.
FAILED: Build did NOT complete successfully (20 packages loaded, 73 targets configured)
    currently loading: @remotejdk17_linux_toolchain_config_repo// ... (13 packages)
    Fetching @local_jdk; fetching
maciej@euler:~/src/bazel_pathdemo$
```
