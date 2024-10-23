# Base image
FROM balenalib/raspberrypi4-64-python:3.9

# Set working directory
WORKDIR /usr/src/app

# Copy the requirements file if you have any, or just the application
COPY . .

# Install required packages
RUN pip install flask

# Start the application
CMD ["python3", "main.py"]
