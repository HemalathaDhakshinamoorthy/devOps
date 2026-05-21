# Use Ubuntu as base image
FROM ubuntu:latest

# Avoid interactive prompts during package installation
ENV DEBIAN_FRONTEND=noninteractive

# Update packages and install Apache2
RUN apt update && \
    apt install -y apache2 && \
    apt clean

# Expose Apache port
EXPOSE 80

# Start Apache automatically when container starts
CMD ["apachectl", "-D", "FOREGROUND"]