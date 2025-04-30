# Use official Python runtime as the base image
FROM python:3.12-slim

# Set the working directory in the container
WORKDIR /app

# Copy all files from the current directory into the container at /app
COPY . /app

# Install dependencies from requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Expose the port Streamlit uses (default is 8501)
EXPOSE 8501

# Command to run the app when the container starts
CMD ["streamlit", "run", "app.py"]
