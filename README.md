# GCP WebApp CI/CD Example

This repository demonstrates a simple CI/CD pipeline for a Web UI application deployed on Google Cloud Platform (GCP) using Cloud Build and Kubernetes.

## Overview

The example includes:
- A basic Web UI application.
- Dockerfile for containerizing the application.
- Kubernetes configurations for deploying the application.
- A Cloud Build configuration for automating the build and deployment process.

## Application

The Web UI application is a simple Python Flask app (you can substitute this with your technology stack) that serves a basic HTML page.

## Structure

```plaintext
├── webapp
│   ├── app.py                 # Application source code
│   ├── Dockerfile             # Dockerfile for building the application container
│   └── requirements.txt       # Python dependencies
├── README.md                  # This README file
├── cloudbuild.yaml            # Cloud Build configuration
├── app-deployment.yaml        # Kubernetes Deployment configuration
└── app-service.yaml           # Kubernetes Service configuration
```
## Setup and Deployment

Prerequisites
- Google Cloud Platform account
- Enabled Google Kubernetes Engine (GKE) and Cloud Build APIs
- Configured gcloud CLI tool

## Steps

1. Clone the repository:
```sh
git clone https://github.com/LF3551/gcp-webapp-cicd-example.git
cd gcp-webapp-cicd-example
```
2. Build and push the Docker image:
This step is automated with Cloud Build when you push changes to the repository. You can also manually build the Docker image and push it to Google Container Registry (GCR).
3. Deploy the application to GKE:
The cloudbuild.yaml file includes steps to deploy the application using kubectl. Make sure your Cloud Build service account has the necessary permissions.
4. Access the application:
After deployment, find the external IP of your service and access the Web UI application in your browser.

## Contributing

Contributions are welcome! Please feel free to submit a pull request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.