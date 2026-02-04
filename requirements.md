# Krishi-Netra Requirements Document

## 1. Project Overview

Krishi-Netra is an AI-powered, voice-first mobile application designed to assist Indian farmers with objective crop quality assessment and fair price estimation. The application addresses critical challenges in agricultural marketing by providing scientific crop grading through computer vision and voice interaction in local languages.

**Project Name**: Krishi-Netra – "Bharat ka Digital Kisan Sathi"  
**Target Users**: Indian farmers with varying literacy levels  
**Primary Platform**: Android mobile application  
**Core Technology**: Computer vision, voice recognition, multilingual NLP

## 2. Problem Statement

### 2.1 Subjective Manual Grading
- Current mandi grading relies on visual inspection by intermediaries
- Inconsistent quality assessment leads to price disputes
- Lack of standardized grading criteria across different markets
- Farmers have limited recourse against biased quality assessments

### 2.2 Language and Usability Barriers
- Existing agricultural apps primarily use English or Hindi interfaces
- Low literacy rates among rural farmers limit app adoption
- Complex user interfaces unsuitable for farmers with limited smartphone experience
- Lack of voice-based interaction in regional languages

### 2.3 Absence of Verified Quality Proof
- No documented evidence of crop quality for farmers
- Difficulty in negotiating fair prices without objective quality metrics
- Limited transparency in the grading process
- Farmers cannot validate quality assessments independently

### 2.4 Price Exploitation via Intermediaries
- Information asymmetry between farmers and buyers
- Lack of real-time market price awareness
- Dependence on middlemen for price discovery
- Limited access to multiple buyer networks

## 3. Objectives

### 3.1 Primary Objectives
- Enable objective crop quality assessment using AI-powered visual analysis
- Provide fair price estimation based on current mandi rates and crop quality
- Improve accessibility through voice-first interface in multiple Indian languages
- Generate verifiable digital quality certificates for farmers

### 3.2 Secondary Objectives
- Reduce dependency on intermediaries for quality assessment
- Increase farmer confidence in market negotiations
- Standardize crop grading across different regions
- Create a digital record of crop quality for future reference

## 4. Stakeholders

### 4.1 Primary Stakeholders
- **Farmers**: End users who capture crop images and receive quality assessments
- **Agricultural Cooperatives**: Organizations that may integrate the platform
- **Development Team**: Engineers, designers, and agricultural experts

### 4.2 Secondary Stakeholders
- **Buyers/Traders**: Potential users of quality certificates for procurement
- **Government Agricultural Departments**: Policy makers and extension officers
- **Platform Administrators**: System operators and data managers

### 4.3 External Stakeholders
- **Mandi Committees**: Source of pricing data and market information
- **Agricultural Research Institutes**: Domain experts for quality parameters
- **Mobile Network Operators**: Infrastructure providers for connectivity
## 5. Functional Requirements

### 5.1 Voice-Driven Crop Image Capture
- **REQ-5.1.1**: System shall support voice commands to initiate camera functionality
- **REQ-5.1.2**: Application shall provide voice guidance for optimal image capture
- **REQ-5.1.3**: System shall accept multiple images per crop sample (minimum 3, maximum 10)
- **REQ-5.1.4**: Application shall validate image quality before processing
- **REQ-5.1.5**: System shall support offline image capture with sync capability

### 5.2 AI-Based Visual Quality Grading
- **REQ-5.2.1**: System shall analyze crop images using computer vision algorithms
- **REQ-5.2.2**: Application shall classify crops into three grades: A+, A, and B
- **REQ-5.2.3**: System shall provide confidence scores for quality assessments
- **REQ-5.2.4**: Application shall support grading for major crops: wheat, rice, cotton, sugarcane
- **REQ-5.2.5**: System shall identify common defects: discoloration, pest damage, moisture content indicators

### 5.3 Fair Price Estimation
- **REQ-5.3.1**: System shall integrate with government mandi price APIs
- **REQ-5.3.2**: Application shall calculate price estimates based on quality grade and current market rates
- **REQ-5.3.3**: System shall provide price ranges rather than fixed values
- **REQ-5.3.4**: Application shall display historical price trends for context
- **REQ-5.3.5**: System shall update pricing data at least twice daily

### 5.4 Multilingual Voice Interaction
- **REQ-5.4.1**: Application shall support voice commands in Hindi, English, and 5 regional languages
- **REQ-5.4.2**: System shall provide voice feedback for all major functions
- **REQ-5.4.3**: Application shall support speech-to-text for crop type selection
- **REQ-5.4.4**: System shall handle voice input with background noise tolerance
- **REQ-5.4.5**: Application shall provide text alternatives for all voice interactions

### 5.5 Digital Quality Certificate Generation
- **REQ-5.5.1**: System shall generate PDF certificates with crop quality details
- **REQ-5.5.2**: Certificate shall include timestamp, location, quality grade, and confidence score
- **REQ-5.5.3**: Application shall embed QR codes for certificate verification
- **REQ-5.5.4**: System shall store certificates locally and in cloud storage
- **REQ-5.5.5**: Certificates shall be shareable via messaging apps and email
## 6. Non-Functional Requirements

### 6.1 Performance
- **REQ-6.1.1**: Image processing shall complete within 30 seconds on mid-range Android devices
- **REQ-6.1.2**: Application startup time shall not exceed 5 seconds
- **REQ-6.1.3**: Voice recognition response time shall be under 3 seconds
- **REQ-6.1.4**: System shall support concurrent processing of up to 100 requests

### 6.2 Scalability
- **REQ-6.2.1**: Backend infrastructure shall support 10,000 daily active users initially
- **REQ-6.2.2**: System shall scale to 100,000 users within 12 months
- **REQ-6.2.3**: Database shall handle 1 million crop assessments annually
- **REQ-6.2.4**: API response times shall remain under 2 seconds at peak load

### 6.3 Security
- **REQ-6.3.1**: All data transmission shall use HTTPS encryption
- **REQ-6.3.2**: User location data shall be anonymized for privacy
- **REQ-6.3.3**: Crop images shall be processed locally when possible
- **REQ-6.3.4**: System shall implement secure API authentication
- **REQ-6.3.5**: Personal data shall comply with Indian data protection regulations

### 6.4 Availability
- **REQ-6.4.1**: System uptime shall be 99.5% during agricultural seasons
- **REQ-6.4.2**: Core functionality shall work offline for image capture and basic grading
- **REQ-6.4.3**: Application shall gracefully handle network interruptions
- **REQ-6.4.4**: System shall provide meaningful error messages in local languages

### 6.5 Accessibility
- **REQ-6.5.1**: Interface shall be usable by farmers with basic smartphone literacy
- **REQ-6.5.2**: Voice commands shall accommodate regional accents and dialects
- **REQ-6.5.3**: Visual elements shall be optimized for outdoor viewing conditions
- **REQ-6.5.4**: Application shall support devices with limited storage (minimum 2GB RAM)
- **REQ-6.5.5**: Font sizes and UI elements shall be accessible for users with visual impairments
## 7. System Constraints

### 7.1 Mobile Camera Quality Limitations
- Image quality dependent on smartphone camera capabilities
- Varying lighting conditions in field environments
- Limited zoom and macro photography capabilities on budget devices
- Potential image blur from hand movement during capture

### 7.2 Internet Connectivity Dependency
- Rural areas may have intermittent network coverage
- Data costs may limit frequent API calls for price updates
- Offline functionality required for core image capture features
- Sync delays when connectivity is restored

### 7.3 AI Model Accuracy Variability
- Computer vision accuracy varies by crop type and condition
- Model performance affected by image quality and lighting
- Regional crop varieties may not be well-represented in training data
- Continuous model updates required for improved accuracy

### 7.4 Device Hardware Limitations
- Processing power constraints on entry-level smartphones
- Limited storage capacity for offline model deployment
- Battery consumption during intensive image processing
- Memory limitations affecting app performance

## 8. Assumptions

### 8.1 User Technology Access
- Target users have Android smartphones with camera functionality
- Users have basic familiarity with smartphone operations
- Devices support minimum Android API level 21 (Android 5.0)
- Users can access mobile data or WiFi connectivity periodically

### 8.2 Infrastructure Availability
- Government mandi price APIs remain accessible and updated
- Mobile network coverage exists in target agricultural regions
- Cloud storage services maintain reliable uptime
- Voice recognition services support required Indian languages

### 8.3 Data and Content
- Mandi price data is updated regularly by government sources
- Crop quality parameters align with existing agricultural standards
- Regional language voice models are available and accurate
- Agricultural experts are available for model validation

### 8.4 Regulatory Environment
- No legal restrictions on AI-based crop quality assessment
- Data privacy regulations remain stable during development
- Agricultural policies support digital innovation initiatives
- No licensing requirements for quality assessment applications

## 9. Out of Scope

### 9.1 B2B Marketplace Functionality
- Direct buyer-seller transaction processing
- Payment gateway integration
- Order management and fulfillment
- Logistics and delivery coordination

### 9.2 Blockchain Traceability
- Immutable crop history tracking
- Supply chain transparency features
- Smart contract implementation
- Distributed ledger technology

### 9.3 Global Pricing Analysis
- International commodity price integration
- Export market price comparison
- Currency conversion and hedging
- Global supply-demand analytics

### 9.4 Legal Certification Claims
- Legally binding quality certificates
- Regulatory compliance certification
- Insurance claim support documentation
- Court-admissible quality evidence

### 9.5 Advanced Agricultural Services
- Crop disease diagnosis and treatment
- Fertilizer and pesticide recommendations
- Weather forecasting and alerts
- Soil testing and analysis integration