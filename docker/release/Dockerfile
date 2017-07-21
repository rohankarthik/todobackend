FROM rohankarthik/todobackend-base:latest
MAINTAINER Rohan Karthik <rohankarthik@outlook.com>


# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse