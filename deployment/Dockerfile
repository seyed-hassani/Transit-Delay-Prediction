# deployment/Dockerfile

FROM public.ecr.aws/lambda/python:3.8

# Install required packages
COPY requirements.txt ./
RUN pip install --upgrade pip && pip install -r requirements.txt

# Copy source files
COPY src/ ./src/
COPY models/ ./models/

# Set the command to your Lambda handler
CMD ["src.train_model.main"]
