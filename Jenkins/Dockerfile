# Use the official Jenkins LTS (Long Term Support) image as the base image
FROM jenkins/jenkins:lts

# Set user to root to install additional tools
USER root

# Install necessary packages
RUN apt-get update && \
    apt-get install -y sudo git curl

# Add Docker (for Jenkins to manage Docker containers) 
RUN curl -fsSL https://get.docker.com/ | sh

# Add the Jenkins user to the docker group
RUN usermod -aG docker jenkins

# Switch back to the Jenkins user
USER jenkins

# Expose the Jenkins web UI port
EXPOSE 8080

# Expose the Jenkins agent port
EXPOSE 50000

# The default CMD is already defined in the base image, no need to specify it
