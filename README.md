# Resume Tracker Monorepo

Welcome to the Resume Tracker monorepo, a comprehensive solution designed to streamline the recruitment process. Our platform facilitates a dynamic interaction between recruiters and candidates, enabling candidates to upload their CVs and recruiters to view and download these CVs with ease.

## Overview

The Resume Tracker application is composed of several microservices, each responsible for a specific segment of the application's functionality. The microservices include:

- **Frontend**: The user interface for both candidates and recruiters.
- **Auth Microservice**: Handles user authentication, including sign-up and login operations.
- **Candidate Microservice**: Manages candidate information, stores details in the database, and uploads CVs to AWS S3.
- **Recruiter Microservice**: Allows recruiters to access candidate information and download CVs using signed URLs from AWS S3.
- **Emailer Microservice**: Listens to an AWS SQS queue for email-related events and sends emails based on the received message payloads.

### Key Features

- **User Authentication**: Secure sign-up and login facilitated by the Auth Microservice.
- **CV Upload and Storage**: Candidates can upload their CVs, which are securely stored in AWS S3.
- **Recruiter Access**: Recruiters can view candidate profiles and download CVs directly.
- **Email Notifications**: Automated email notifications for various events, such as successful sign-up, CV uploads, and downloads.
