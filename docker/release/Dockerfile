FROM nmiletic/todobackend-base:latest
MAINTAINER Nemanja Miletic <nemanja@nemanjamiletic.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse
