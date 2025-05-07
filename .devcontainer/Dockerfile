FROM ubuntu:22.04

# Update package lists and install required packages
RUN apt-get update && apt-get install -y \
    curl \
    wget \
    git \
    software-properties-common \
    openjdk-8-jdk \
    maven

# Install Golang
RUN wget https://go.dev/dl/go1.23.0.linux-amd64.tar.gz && \
    tar -C /usr/local -xzf go1.23.0.linux-amd64.tar.gz && \
    rm go1.23.0.linux-amd64.tar.gz

# Set Go environment variables
ENV PATH=$PATH:/usr/local/go/bin
ENV GOPATH=/go
ENV GOROOT=/usr/local/go

# Verify installations
RUN java -version && \
    mvn --version && \
    go version

# Clean up
RUN apt-get clean && \
    rm -rf /var/lib/apt/lists/*
