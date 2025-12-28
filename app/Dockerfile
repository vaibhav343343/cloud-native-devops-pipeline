# Base Python image
FROM python:3.12-slim

# Working directory inside container
WORKDIR /app

# Copy application code
COPY app.py /app/

# Install Flask
RUN pip install flask

# Expose application port
EXPOSE 5000

# Start the application
CMD ["python", "app.py"]

