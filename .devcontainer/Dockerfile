# Use the official Codespaces Ruby image
FROM mcr.microsoft.com/vscode/devcontainers/ruby:3

# Install any additional dependencies you may need
# For example, if you need a specific gem, you can install it here
# RUN gem install your_gem_name

# Set the default user to root for Codespaces
USER root

# Update and install the latest Ruby version
RUN apt-get update && apt-get install -y \
    ruby-full

# Clean up apt-get to reduce image size
RUN apt-get clean && rm -rf /var/lib/apt/lists/*

# Switch back to the non-root user
USER codespace
