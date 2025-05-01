# Use the base image for Rust
FROM mcr.microsoft.com/devcontainers/rust:1-bullseye

# Install additional tools
RUN apt-get update && apt-get install -y \
    build-essential \
    libssl-dev \
    pkg-config \
    && apt-get clean

# Set default user to vscode
USER vscode

# Set working directory
WORKDIR /workspace
