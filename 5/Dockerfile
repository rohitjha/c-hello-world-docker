# Dockerfile
FROM alpine as build
COPY hello.c .
RUN apk add --no-cache gcc musl-dev && \
    gcc -o hello hello.c

FROM alpine
COPY --from=build hello .
CMD ["./hello"]
