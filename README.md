# CSCE412 Project 5 - Secure Website

This project is a secure static website hosted on AWS using S3, CloudFront, and Route 53.

## Features
- Secure HTTPS connection using AWS Certificate Manager
- Static website hosting with Amazon S3
- Global content delivery with CloudFront
- Custom domain routing with Route 53
- Automatic deployment using CodePipeline

## CI/CD Pipeline
The website automatically updates when changes are pushed to GitHub. AWS CodePipeline deploys the files to S3 and invalidates the CloudFront cache so updates appear immediately.

## How to Update
1. Edit website files locally
2. Run:
   git add .
   git commit -m "update"
   git push
3. Pipeline runs automatically and updates the site
