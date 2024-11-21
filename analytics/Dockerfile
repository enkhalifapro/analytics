# Use the official Alpine base image
FROM python:3.9-alpine

# Set environment variables
ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1

# Set work directory
WORKDIR /analytics

# Install dependencies
COPY requirements.txt /analytics/
RUN pip install --no-cache-dir -r requirements.txt

# Copy project
COPY . /analytics/

# Expose the port your application runs on
EXPOSE 5153

# Run the application
CMD ["python", "app.py"]
