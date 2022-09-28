# Security Scans on GCP

This repo is created to demontrate how to setup **Security scans on GCP** and covers the below steps for Python and NodeJs.

 1. Audit the packages installed
 2. Security scans by Sonar scanner
 3. Unit test 
 4. Code coverage
 5. Safety check for vulnerabilities (Python)
 6. Snyk.io scan for vulnerability check

## Files

 - *Dockerfile*
 - *cloudbuild.yaml*
 - *package.json*
 - *security-scans-nodejs.yaml*
 - *security-scans-python.yaml*
 
## Dependencies

 - *gcp-sonar-scanner*

Clone this Repo and follow the readme file for the deployment.

## How trigger the pipeline automatically?
Enable Google Cloud Build for your repository. 

**Github > Market place > Google Cloud Build App > Enable.**

Setup build triggger under Google Cloud Project under Cloud Build for the repository.

## Tokens & Secrets
Maintain Tokens and secrets in Google Cloud Secret Manager. Refer cloudbuild.yaml

## Command
Clone the Repo and run the below command on GCP Cloud shell.

    gcloud builds submit --config=cloudbuild.yaml
