# Project Overview

I created MedTracker to be a serverless AWS application designed to help me consolidate all the various medical information from multiple 
healthcare providers. It also allows me to generate visit-specific reports that show all of my health visits and records that have happened
since the last time I saw that specific doctor.

The application provides secure authentication, medical record management, document storage, visit tracking, and printable physician reports. 
While it is a working application at this point and I have used it at recent doctors appointments, it is also a work in progress.

## Motivation
I am diabetic and I have a lot of doctors.  Managing health data across all of these different providers many who use completely different 
portals is fragmented and does not allow doctors to see what each other are doing.
This project explores how to design a secure, scalable personal health record system while remaining cost-conscious for individual users.

## Architecture
User  
 │  
 ▼  
React Frontend  
(AWS Amplify)  
 │  
 ▼  
Amazon Cognito  
 │  
 ▼  
API Gateway  
 │  
 ▼  
Lambda  
 ├── DynamoDB  
 └── S3

## AWS Services Used
- AWS Amplify
- Amazon Cognito
- Amazon API Gateway
- AWS Lambda
- Amazon DynamoDB
- Amazon S3
- GitHub

## Cost Optimization
> The architecture intentionally avoids always-on infrastructure
> (e.g., EC2, ALB, RDS) to minimize cost during early development.

## Key Features
- Secure user authentication
- Medical record management
- Visit tracking
- Document upload/download
- Chronological reporting
- Printable physician summaries

## Technical Challenges Solved
- Cognito authentication integration
- Secure API authorization
- S3 document management
- Browser upload troubleshooting
- Report generation and printing
- DynamoDB single-table design

## Roadmap/Future Enhancements
- Search and better filtering
- Update/consolidate visits
- Dashboard analytics
- Improve printable summary layouts
- AI?  Quarterly summaries?


