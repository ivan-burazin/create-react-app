# Use the official Node.js image as the base image
FROM mcr.microsoft.com/vscode/devcontainers/javascript-node:14

# Install additional packages if needed
RUN sudo apt-get update && sudo apt-get install -y \
    git \
    curl

# Set the working directory
WORKDIR /workspace

# Copy the project files
COPY . /workspace

# Expose port 3000 for the React development server
EXPOSE 3000

# Default command to run (can be overridden in devcontainer.json)
CMD ["npm", "start"]
