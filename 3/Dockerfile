# Dockerfile
FROM ubuntu
COPY hello.c .
RUN apt-get update && \
    apt-get install -y gcc-10 && \
    gcc-10 -o hello hello.c
CMD ["./hello"]
