# Dockerfile
FROM gcc as build
COPY hello.c .
RUN gcc -o hello hello.c -static

FROM busybox
COPY --from=build hello .
CMD ["./hello"]
