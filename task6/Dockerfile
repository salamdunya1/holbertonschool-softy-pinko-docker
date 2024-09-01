# Use the latest Ubuntu image as the base
FROM ubuntu:latest

#Update and upgrade APT packages
RUN apt-get update && apt-get upgrade -y

#Install Python3 and pip3
RUN apt-get install -y python3 python3-pip

#Remove the EXTERNALLY-MANAGED file if necessary
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask using pip3
RUN pip3 install flask

# Install Flask-cors using pip3
RUN pip3 install flask flask-cors

# Set the working directory
WORKDIR /app

# Copy the api.py file to the Docker image
COPY ./api.py /app/api.py

#Run the Flask app
CMD echo "Hello, World!"
