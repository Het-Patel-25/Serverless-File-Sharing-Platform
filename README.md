# Serverless File Sharing Platform

## Project Description
The Serverless File Sharing Platform allows users to securely upload and download files through a simple HTTP API. It uses AWS Lambda for serverless compute, API Gateway for RESTful APIs, and Amazon S3 for scalable object storage.

## Use Cases
* **File Sharing:** Upload files via POST and retrieve them via GET.
* **File Distribution:** Generate shareable file links for distribution.
* **Collaborative Work:** Share documents and resources securely with teams.

## Project Architecture
![Project Architecture Diagram](architecture.png)

## Steps to Build the Project

### Prerequisites
* AWS account with Lambda, API Gateway, and S3 permissions.

### Deployment Steps
1. Create an S3 bucket for uploads.
2. Create the `UploadFunction` Lambda to save files to S3.
3. Create the `DownloadFunction` Lambda to read files from S3.
4. Configure API Gateway routes for upload and download.

## Files in this Repository
* `UploadFunction.py` — Lambda handler for uploading files to S3.
* `DownloadFunction.py` — Lambda handler for downloading files from S3.
* `README.md` — Project overview and deployment guidance.
