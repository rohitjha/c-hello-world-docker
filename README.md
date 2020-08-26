# c-hello-world-docker

Building a tiny Docker image that run a "Hello, World!" C program, step-by-step.

For more details, check out this blog post: <https://www.rohitjha.dev/posts/0x01-minimizing_docker_image_sizes/>

## Comparison

| Image             | Size          |
| :-------------    | :-----------: |
| `gcc` base image  | 1.19GB        |
| `ubuntu` base image   | 244MB     |
| `ubuntu` base image, multi-stage build  | 73.9MB     |
| `alpine` base image, multi-stage build, statically-linked using glibc  | 6.52MB     |
| `alpine` base image, multi-stage build, statically-linked using musl libc  | 5.59MB     |
| `busybox:glibc` base image, multi-stage build  | 5.22MB     |
| `busybox` base image, multi-stage build, statically-linked using glibc  | 2.17MB     |
| `scratch` base image, multi-stage build, statically-linked using glibc  | 945KB     |
| `scratch` base image, multi-stage build, statically-linked using musl libc  | 96.3KB     |
