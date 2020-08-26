# Dockerfile
FROM alpine as build
COPY hello.c .
RUN apk add --no-cache gcc musl-dev && \
    gcc -o hello hello.c -static

FROM scratch
COPY --from=build hello .
CMD ["./hello"]
