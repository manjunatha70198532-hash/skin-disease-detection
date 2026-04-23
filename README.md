# DermaVision AI

## Project Title
DermaVision AI - Intelligent Dermatology Diagnostic System

## Problem Statement
Skin diseases affect millions of people worldwide, yet access to dermatological expertise remains limited, especially in rural and underserved areas. Traditional diagnosis requires in-person consultations with dermatologists, which can be time-consuming, expensive, and often delayed. Early detection and proper identification of skin conditions are critical for effective treatment, but many people lack immediate access to professional medical guidance. There is a need for an accessible, AI-powered preliminary screening tool that can help individuals identify potential skin conditions and connect them with appropriate healthcare resources.

## Description
DermaVision AI is a comprehensive web-based dermatology diagnostic application that leverages advanced artificial intelligence to analyze skin images and provide detailed medical insights. The system allows users to upload images of skin conditions, receives AI-powered analysis with confidence scores, and provides comprehensive information about the detected condition including causes, symptoms, treatments, and prevention measures.

Key capabilities include:
- Real-time AI-powered skin disease detection using computer vision
- Detailed diagnostic reports with medical information
- Interactive AI chatbot for personalized dermatological guidance
- Analytics dashboard with confidence metrics and health scores
- Clinic directory and appointment booking system
- Complete history tracking and PDF report generation
- Multi-language support and accessibility features
- Customizable themes and user preferences

The application serves as a preliminary screening tool to help users understand their skin conditions before consulting with healthcare professionals.

## Proposed Solution
DermaVision AI addresses the accessibility gap in dermatological healthcare through a multi-layered AI-driven approach:

1. **Instant AI Analysis**: Users upload skin images which are analyzed by Groq's advanced vision model (Meta Llama-4 Scout 17B) to identify potential skin diseases with confidence scores and probability distributions across multiple conditions.

2. **Comprehensive Medical Information**: The system provides detailed information about detected conditions including causes, symptoms, effects, prevention methods, recommended treatments, and medications.

3. **Intelligent Chatbot Assistant**: A specialized dermatology AI (Llama-3.3 70B) offers contextual, personalized advice based on the user's diagnosis, available 24/7 for follow-up questions.

4. **Healthcare Integration**: Built-in clinic finder and appointment booking system connects users with nearby dermatology specialists, bridging the gap between AI screening and professional medical care.

5. **Data Persistence & Analytics**: All analyses are stored locally with visual analytics, enabling users to track their skin health over time and share reports with healthcare providers.

6. **Accessibility & Customization**: Voice support, multi-language options, and customizable themes ensure the application is accessible to diverse user populations.

The solution operates entirely on a local-first architecture with SQLite database, ensuring data privacy while providing enterprise-grade AI analysis capabilities.

## Tech Stack

**Frontend:**
- React 19.0 with TypeScript
- TailwindCSS 4.1
- Motion (Framer Motion) for animations
- Chart.js for data visualization
- Lucide React icons
- jsPDF + html2canvas for PDF generation

**Backend:**
- Node.js with Express.js 4.21
- SQLite (better-sqlite3)
- Multer for file uploads

**AI/ML:**
- Groq SDK
- Meta Llama-4 Scout 17B (Vision Analysis)
- Llama-3.3 70B Versatile (Chat Assistant)

**Development:**
- Vite 6.2 (Build tool)
- TypeScript 5.8
- React DOM 19.0
