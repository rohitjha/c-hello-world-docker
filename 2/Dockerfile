# Dockerfile
FROM ubuntu
COPY hello.c .
RUN apt-get update
RUN apt-get install -y gcc-10
RUN gcc-10 -o hello hello.c
CMD ["./hello"]
