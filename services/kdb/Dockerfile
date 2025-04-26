FROM ubuntu:22.04

# Install minimal dependencies
RUN apt-get update && apt-get install -y \
    libgomp1 \
    libssl3 \
    curl \
    && rm -rf /var/lib/apt/lists/*

# Create KDB+ working directory
RUN mkdir -p /opt/kdb

# Copy files into the container
COPY . /opt/kdb/

# Set environment variables
ENV QHOME=/opt/kdb
ENV PATH="$QHOME/l64:$PATH"

# Expose the default q port
EXPOSE 5000

# Start the q binary
CMD ["q"]