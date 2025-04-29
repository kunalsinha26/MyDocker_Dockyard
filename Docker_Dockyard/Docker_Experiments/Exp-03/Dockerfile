# Use a base Python image
FROM python:3-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the application code into the container
COPY app.py .

# Run the Python application
CMD ["python","app.py", "--server.port=8503", "--server.enableCORS=false"]
