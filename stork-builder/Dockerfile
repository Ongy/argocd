FROM alpine:latest

# Install bash, curl to fetch and run the repository setup script
RUN apk add --no-cache bash curl

# Set up Cloudsmith repository and install the Stork server
RUN curl -1sLf 'https://dl.cloudsmith.io/public/isc/stork/cfg/setup/bash.alpine.sh' | bash && \
    apk add --no-cache isc-stork-server

# Expose Stork REST API default port
EXPOSE 8080

# Run stork-server. CMD will search for it in PATH.
CMD ["stork-server"]
