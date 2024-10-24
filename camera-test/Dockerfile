# Base image
FROM balenalib/%%BALENA_MACHINE_NAME%%-debian

# Install dependencies
RUN apt-get update && apt-get install -y \
    python3 \
    python3-pip \
    libopencv-dev \
    python3-opencv \
    && rm -rf /var/lib/apt/lists/*

# Set up working directory
WORKDIR /usr/src/app

# Copy test script
COPY test_camera.py .

# Set entrypoint to execute the test script
CMD ["python3", "test_camera.py"]
