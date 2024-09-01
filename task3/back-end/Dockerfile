# Use the latest Ubuntu image
FROM ubuntu:latest

# Update and upgrade the system
RUN apt-get update && apt-get upgrade -y

# Install Python3 and pip3
RUN apt-get install -y python3 python3-pip

# Remove EXTERNALLY-MANAGED file to prevent installation issues
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask using pip3
RUN pip3 install flask

# Install flask-cors using pip3
RUN pip3 install flask-cors

# Set the working directory
WORKDIR /app

# Copy the Python file into the Docker image
COPY ./api.py /app/api.py

# Expose the port that the Flask app runs on
EXPOSE 5000

# Run the Flask application
CMD ["python3", "api.py"]
