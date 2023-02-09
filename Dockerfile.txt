# Use Ubuntu 22.04 as the base image
FROM ubuntu:22.04 

# Update the package repository and install Java 1.8
RUN apt-get update && apt-get install -y openjdk-8-jdk 

# Verify the Java version
RUN java -version 

# Set the default command to run when starting the container
CMD ["/bin/bash"]