# Use Python 3.10 base image
FROM python:3.10

# Set working directory
WORKDIR /django

# Copy requirements.txt file to the working directory
COPY requirements.txt /django/

# Upgrade pip and install dependencies
RUN pip install --upgrade pip && \
    pip install -r requirements.txt

# Copy the rest of the application files
COPY . /django

# Set environment variables (if needed)
# ENV ...

# Command to run the application (adjust as necessary)
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
