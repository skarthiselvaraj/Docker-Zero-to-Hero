FROM ubuntu:latest

# Update package lists
RUN apt-get update

# Install Python and pip
RUN apt-get install -y python3 python3-pip

# Install Python dependencies
COPY requirements.txt /app/requirements.txt
RUN pip install --break-system-packages -r /app/requirements.txt


# Change directory to /devops
WORKDIR /app/devops
