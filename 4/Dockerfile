# Dockerfile
FROM gcc as build
COPY hello.c .
RUN gcc -o hello hello.c

FROM ubuntu
COPY --from=build hello .
CMD ["./hello"]
