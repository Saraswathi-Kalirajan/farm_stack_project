# Use official Python image
FROM python:3.11-slim

# Disable .pyc files and enable unbuffered logging
ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1

# System dependencies
RUN apt-get update && apt-get install -y --no-install-recommends \
    build-essential \
    gcc \
    python3-dev \
    libffi-dev \
    libssl-dev \
    && rm -rf /var/lib/apt/lists/*

# Set working directory
WORKDIR /usr/src/app

# Copy dependencies first
COPY requirements.txt .

# Install Python dependencies
RUN pip install --upgrade pip setuptools wheel \
    && pip install --no-cache-dir -r requirements.txt

# Copy the entire project into the image
COPY . .

# Add src to PYTHONPATH
ENV PYTHONPATH="/usr/src/app/src"

# Fix: Expose FastAPI port
EXPOSE 8000

# Fix: Start FastAPI on port 8000
CMD ["uvicorn", "src.server:app", "--host", "0.0.0.0", "--port", "8000"]