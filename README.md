
# AWS Face Recognition System

This project is a Flask web application that uses AWS Rekognition for real-time face recognition and AWS S3 for image storage along with DynamoDB for metadata management.


## Features

- Upload images to an AWS S3 bucket.
- Register new persons with their photos.
- Recognize faces using AWS Rekognition.
- Capture images directly from the webcam.


## Tech Stack

**Flask:** Web framework for Python.

**AWS Rekognition:** Service for face detection and recognition.

**AWS S3:** Object storage for images.

**Boto3:** AWS SDK for Python.

**WTForms:** Forms handling library for Flask.

**PIL (Pillow):** Python Imaging Library.


## Setup

**Environment Variables**

Create a .env file in the root directory of the project to securely manage your environment variables. 
Add the following variables:

SECRET_KEY = your_secret_key_here

AWS_ACCESS_KEY_ID = your_aws_access_key_id

AWS_SECRET_ACCESS_KEY = your_aws_secret_access_key

AWS_REGION = us-east-1


## Dependencies

Install the dependencies by running:
```bash
pip install -r requirements.txt
```


## AWS Setup

S3 Bucket: Create a S3 bucket with an unique name.

Rekognition Collection: Create a Rekognition collection named famouspersons.

DynamoDB Table: Create a DynamoDB table named facerecognition with a primary key RekognitionId (string).
## Run Locally

Start the Flask development server

```bash
  python main.py
```

Open a browser and navigate to http://localhost:5000 to access the application.
