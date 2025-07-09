# Base image
FROM mcr.microsoft.com/devcontainers/base:ubuntu

# Use an environment variable to conditionally install the fish shell feature
ARG USE_FISH=false
RUN if [ "$USE_FISH" = "true" ]; then \
    curl -fsSL https://raw.githubusercontent.com/meaningful-ooo/devcontainer-features/main/install.sh | bash -s -- fish:2; \
fi
