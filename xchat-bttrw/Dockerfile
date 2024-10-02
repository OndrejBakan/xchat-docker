# Stage 1: Build in Ubuntu
FROM ubuntu:22.04 as builder

# Install dependencies for building the project
RUN apt-get update && apt-get install -y \
    build-essential \
    libcurl4-openssl-dev \
    git \
    cmake

# Set working directory
WORKDIR /app

COPY ./src /app

RUN ./mkreadme || echo "mkreadme failed"

# RUN chmod +x /app/mkreadme

# RUN make -k
