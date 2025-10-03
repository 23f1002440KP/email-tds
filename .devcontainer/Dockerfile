# Use base Ubuntu image from devcontainers
FROM mcr.microsoft.com/devcontainers/base:ubuntu

# Install Python3, pip, and any other dependencies
RUN apt-get update && \
    apt-get install -y python3 python3-pip && \
    update-alternatives --install /usr/bin/python python /usr/bin/python3 10 && \
    python --version

# Install required Python package fastapi globally
RUN python -m pip install --no-cache-dir fastapi
