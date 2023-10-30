# Use a base image with Python pre-installed
FROM python:3.8

# Set the working directory inside the container
WORKDIR /app

# Copy the application files into the container
COPY requirements.txt /app
COPY app.py /app
# Install Flask (since it's not in requirements.txt for this example)
RUN pip install -r requirements.txt

# Expose the port your Flask app will run on
EXPOSE 5000

# Define the command to start the Flask application
CMD ["python", "app.py"]
