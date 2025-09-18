# Use the latest Ubuntu image as base
FROM ubuntu:latest

# Prevent interactive prompts during apt operations
ENV DEBIAN_FRONTEND=noninteractive

# Update APT and upgrade installed packages
RUN apt-get update && apt-get upgrade -y

# Default command: echo "Hello, World!"
CMD ["echo", "Hello, World!"]

