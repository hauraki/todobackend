FROM hauraki/todobackend-base:latest
MAINTAINER Norbert Stein <norbert@hauraki.de>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse