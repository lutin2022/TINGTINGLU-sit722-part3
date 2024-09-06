
# Dockerfile for inventory_management microservice

# Use an official Python runtime as a parent image
FROM python:3.11.4

# Root Directory
WORKDIR /inventory_management

# Copies the source code for this microservice into the image
COPY ./* .

# Set Environment Variable
ENV DATABASE_URL=postgresql://tingtinglu_sit722_part3_user:iuo7XJ1Hiuw94jOeIhireIR2T08bysuk@dpg-crbtpa5svqrc73f44tq0-a.oregon-postgres.render.com/tingtinglu_sit722_part3

# Build Command
RUN pip install -r requirements.txt

# Start command
CMD uvicorn main:app --host 0.0.0.0 --port $PORT