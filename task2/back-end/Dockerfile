FROM ubuntu:latest

ENV DEBIAN_FRONTEND=noninteractive

# Update + upgrade and install Python3 + pip3
RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y python3 python3-pip && \
    rm -f /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask via pip3 (not apt)
RUN pip3 install flask

# Work in /app and copy api.py
WORKDIR /app
COPY api.py .

# Document the port
EXPOSE 5252

# Run the API
CMD ["python3", "api.py"]

