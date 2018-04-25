FROM clayton949/todobackend-base:latest
MAINTAINER Clayton Wagner <clayton@wagneremail.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
	pip install --no-index -f /wheelhouse todobackend && \
	rm -rf /wheelhouse