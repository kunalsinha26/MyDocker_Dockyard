FROM python:3-slim

# Install system dependencies
RUN apt-get update && apt-get install -y gcc libpq-dev

# Install Python packages
RUN pip install streamlit psycopg2

# Then copy your app files
COPY . /app
WORKDIR /app

# Expose your desired port
EXPOSE 8504

# Command to run the app
CMD ["streamlit", "run", "stream.py", "--server.port=8504", "--server.address=0.0.0.0"]
