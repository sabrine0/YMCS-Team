# Use the official Python image as your base image
FROM python:3.8

# Set working directory to /usr/src/app
WORKDIR /usr/src/app

# Copy the contents of the current local directory into the container's working directory
COPY . .

# Install any required dependencies using pip
RUN pip install --no-cache-dir -r requirements.txt

# Expose the port on which your application will run (8000 in this case)
EXPOSE 8000

# Use uvicorn to run your FastAPI app
CMD ["uvicorn", "api:app", "--host", "0.0.0.0", "--port", "8000", "--reload"]
