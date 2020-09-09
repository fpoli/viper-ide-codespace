FROM mcr.microsoft.com/vscode/devcontainers/rust:1

# Install Java
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends default-jdk \
    && rm -rf /var/lib/apt/lists/*
ENV JAVA_HOME /usr/lib/jvm/default-java
ENV LD_LIBRARY_PATH $JAVA_HOME/lib/server/
