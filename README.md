# Krishi-Netra
**Bharat ka Digital Kisan Sathi**

An AI-powered, voice-first agricultural application that empowers Indian farmers with objective crop quality assessment and fair pricing insights.

## Problem Statement

Indian farmers face significant challenges in the traditional mandi system:

- **Subjective Manual Grading**: Crop quality assessment relies on manual inspection by mandi officials, leading to inconsistent and potentially biased evaluations
- **Language and Digital Barriers**: Farmers struggle with technology interfaces that require typing or navigation in unfamiliar languages
- **Lack of Quality Documentation**: Without standardized quality proof, farmers often receive unfair pricing for their produce
- **Information Asymmetry**: Limited access to real-time market data and pricing trends puts farmers at a disadvantage during negotiations

## Solution Overview

Krishi-Netra addresses these challenges through:

- **Voice-Driven Interface**: Farmers can interact with the app using natural speech in their preferred language
- **Computer Vision Analysis**: AI-powered crop quality assessment using smartphone cameras
- **Objective Grading System**: Standardized quality evaluation before reaching the mandi
- **Market Intelligence**: Integration with mandi data to provide fair price estimates

## Key Features

### Core Features
- **Voice-Driven Crop Image Capture**: Hands-free operation with voice commands for image capture and navigation
- **AI-Based Quality Grading**: Computer vision analysis providing standardized grades (A+, A, B)
- **Fair Price Estimation**: Real-time pricing insights based on current mandi data and crop quality
- **Digital Quality Certificate**: PDF generation with crop details, grade, and timestamp for mandi presentation
- **Multilingual Voice Interface**: Support for multiple Indian languages to ensure accessibility

### Future Enhancements
- **B2B Direct Marketplace**: Connect farmers directly with buyers based on quality grades
- **Scheme Eligibility Assistant**: Voice-guided assistance for government agricultural schemes
- **Global Price Trends**: International market insights for export-quality produce
- **QR-Based Traceability**: End-to-end crop tracking from farm to consumer

## Tech Stack

### Frontend
- React Native for cross-platform mobile development
- Voice recognition and synthesis libraries
- Camera integration for image capture

### Backend
- Node.js with Express framework
- RESTful API architecture
- Authentication and user management

### AI/ML
- Computer vision models for crop quality assessment
- Natural language processing for voice commands
- TensorFlow/PyTorch for model deployment

### Cloud Services (AWS)
- EC2 for application hosting
- S3 for image and document storage
- Lambda for serverless processing
- RDS for structured data storage
- API Gateway for service orchestration

## High-Level Workflow

1. **Voice Input**: Farmer initiates crop assessment using voice commands
2. **Image Capture**: Guided camera capture of crop samples
3. **AI Analysis**: Computer vision model processes images for quality assessment
4. **Grade Assignment**: System assigns standardized quality grade (A+, A, B)
5. **Price Estimation**: Integration with mandi data provides fair price range
6. **Certificate Generation**: PDF quality certificate created with all details
7. **Mandi Presentation**: Farmer presents digital certificate for transparent pricing

## Installation & Setup

### Prerequisites
- Node.js (v16 or higher)
- React Native development environment
- AWS account for cloud services

### Environment Variables
```
AWS_ACCESS_KEY_ID=your_aws_access_key
AWS_SECRET_ACCESS_KEY=your_aws_secret_key
AWS_REGION=your_aws_region
DATABASE_URL=your_database_connection_string
JWT_SECRET=your_jwt_secret
MANDI_API_KEY=your_mandi_data_api_key
```

### Setup Steps
1. Clone the repository
2. Install dependencies: `npm install`
3. Configure environment variables
4. Set up AWS services and database
5. Run development server: `npm run dev`
6. Deploy ML models to cloud infrastructure

## Future Scope

- **Expansion to Additional Crops**: Extend AI models to cover more crop varieties
- **Integration with Government Systems**: Direct connection with agricultural department databases
- **Blockchain Integration**: Immutable quality records for enhanced traceability
- **IoT Sensor Integration**: Real-time field condition monitoring
- **Cooperative Integration**: Tools for farmer producer organizations
- **Financial Services**: Credit scoring based on crop quality history

## Team Information

This project is developed to support Indian farmers in achieving fair pricing through technology-enabled transparency in crop quality assessment. The solution focuses on accessibility, accuracy, and practical implementation in rural agricultural contexts.

---

**Note**: This application aims to assist farmers with crop quality assessment. While the AI models are trained on extensive datasets, farmers should use the results as guidance alongside traditional assessment methods.