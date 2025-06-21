FROM python:3.9-slim

WORKDIR /app

# update dependencies

RUN apt update -y && rm -rf /var/lib/apt/lists/*

# Copy requirements file and install dependencies
COPY . .

RUN pip install --no-cache-dir -r requirements.txt

# Expose the application port
EXPOSE 5000

# Command to run the Flask application
CMD ["python", "app.py"]

# Note: Ensure that your Flask app is set to run on host '

