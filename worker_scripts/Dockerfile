# Use an official Python runtime as a parent image
FROM python:3.8-slim

# Set the working directory in the container
WORKDIR /usr/src/app

# Copy the current directory contents into the container
COPY . .

# Expose port 8000
EXPOSE 8000

# Run the Python HTTP server
CMD ["python", "-m", "http.server", "8000"]
