# Use the official Python image as a base image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy the contents of the spendvest_backend_py directory into the container at /app
COPY spendvest_backend_py /app

# Install any needed dependencies specified in requirements.txt
RUN pip install --no-cache-dir -r /app/requirements.txt

# Make port 5000 available to the world outside this container
EXPOSE 5080

# Define the command to run the Flask application
CMD ["python", "/app/app.py"]
