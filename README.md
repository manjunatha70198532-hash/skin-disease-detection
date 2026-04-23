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

# 🩺 DermaVision AI - Advanced Dermatology Diagnostic System

A cutting-edge AI-powered dermatology diagnostic application that leverages computer vision and large language models to analyze skin images, provide medical insights, and connect users with healthcare professionals.

![Version](https://img.shields.io/badge/version-4.0.2-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![React](https://img.shields.io/badge/React-19.0-61dafb)
![Node](https://img.shields.io/badge/Node.js-Express-green)

## ✨ Features

### 🤖 AI-Powered Analysis
- **Vision Analysis**: Upload skin images for instant AI-powered dermatological diagnosis
- **Multi-Condition Detection**: Identifies various skin conditions with confidence scores
- **Detailed Reports**: Comprehensive information including causes, symptoms, treatments, and prevention
- **Probability Distribution**: Shows likelihood of multiple conditions

### 💬 Intelligent ChatBot
- **DermaBot**: Specialized dermatology AI assistant
- **Context-Aware**: Chat responses based on your diagnosis
- **Professional Advice**: Empathetic, medical-grade guidance
- **Always Available**: 24/7 instant responses

### 📊 Analytics & Insights
- **Visual Analytics**: Interactive charts and graphs
- **Confidence Metrics**: Detailed breakdown of AI certainty
- **Health Score**: Overall skin health assessment
- **Historical Trends**: Track changes over time

### 🏥 Healthcare Integration
- **Clinic Directory**: Browse nearby dermatology clinics
- **Appointment Booking**: Schedule appointments directly
- **Doctor Finder**: Location-based specialist recommendations
- **Medical Records**: Complete history of all analyses

### 🎨 User Experience
- **Multiple Themes**: Cyberpunk, scanner, medical, gradient, galaxy wallpapers
- **Voice Support**: Text-to-speech for accessibility
- **Multi-Language**: English and Kannada support
- **PDF Reports**: Download professional diagnostic reports
- **Smooth Animations**: Beautiful, responsive UI with motion effects

## 🏗️ Architecture

### System Overview

```
┌─────────────────────────────────────────────────────────────┐
│                      Frontend (React)                        │
│  ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────────┐   │
│  │Dashboard │ │ History  │ │Analysis  │ │Clinics/Books │   │
│  └──────────┘ └──────────┘ └──────────┘ └──────────────┘   │
└────────────────────────┬────────────────────────────────────┘
                         │ REST API
┌────────────────────────▼────────────────────────────────────┐
│                  Backend (Express.js)                        │
│  ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────────┐   │
│  │ /analyze │ │  /chat   │ │ /history │ │ /appointments│   │
│  └──────────┘ └──────────┘ └──────────┘ └──────────────┘   │
└────────┬──────────────┬──────────────────────┬──────────────┘
         │              │                      │
    ┌────▼────┐    ┌────▼────┐          ┌─────▼─────┐
    │ Groq AI │    │ SQLite  │          │  File Sys │
    │  Vision │    │   DB    │          │  Uploads  │
    └─────────┘    └─────────┘          └───────────┘
```

### Tech Stack

**Frontend:**
- ⚛️ React 19.0 with TypeScript
- 🎨 TailwindCSS 4.1 for styling
- 🎭 Motion (Framer Motion) for animations
- 📊 Chart.js + react-chartjs-2 for visualizations
- 🎯 Lucide React for icons
- 📄 jsPDF + html2canvas for PDF generation

**Backend:**
- 🚀 Express.js 4.21 web framework
- 💾 better-sqlite3 for database
- 📤 Multer for file uploads
- 🔌 Groq SDK for AI integration

**AI Models:**
- 👁️ Meta Llama-4 Scout 17B (Vision Analysis)
- 💬 Llama-3.3 70B Versatile (Chat Assistant)

## 🚀 Getting Started

### Prerequisites

- **Node.js**: v18.0 or higher
- **npm**: v8.0 or higher
- **Groq API Key**: Get one at [console.groq.com](https://console.groq.com)

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd dermavision-ai
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment variables**
   ```bash
   # Create .env file from example
   cp .env.example .env
   
   # Edit .env and add your Groq API key
   # IMPORTANT: Never commit .env to version control!
   GROQ_API_KEY=your_actual_groq_api_key_here
   ```
   
   ⚠️ **Security Warning**: Your `.env` file contains sensitive API keys and is already listed in `.gitignore`. Never share or commit this file to GitHub!

4. **Start the development server**
   ```bash
   npm run dev
   ```

5. **Open your browser**
   Navigate to `http://localhost:3000`

### Build for Production

```bash
npm run build
npm start
```

## 📖 API Documentation

### Endpoints

#### 🔍 Health Check
```
GET /api/health
```
Returns server status and API key configuration.

#### 📸 Image Analysis
```
POST /api/analyze
Content-Type: multipart/form-data

Body:
  - image: File (required)

Response:
{
  "disease": "string",
  "confidence": number,
  "description": "string",
  "causes": "string",
  "effects": "string",
  "symptoms": "string",
  "prevention": "string",
  "medicines": "string",
  "treatment": "string",
  "probabilities": { "ConditionA": number, ... }
}
```

#### 💬 Chat Assistant
```
POST /api/chat
Content-Type: application/json

Body:
{
  "message": "string",
  "context": "string (optional)"
}

Response:
{
  "reply": "string"
}
```

#### 📂 Upload Image
```
POST /api/upload
Content-Type: multipart/form-data

Body:
  - image: File (required)

Response:
{
  "image_url": "/uploads/filename.jpg"
}
```

#### 📚 History Management

**Get all records:**
```
GET /api/history

Response: Array of PredictionResult objects
```

**Save new record:**
```
POST /api/history
Content-Type: application/json

Body: PredictionResult object

Response: Saved object with ID
```

**Delete record:**
```
DELETE /api/history/:id

Response: { "success": true }
```

**Get shared prediction:**
```
GET /api/prediction/:id

Response: PredictionResult object
```

#### 📅 Appointments

**Book appointment:**
```
POST /api/appointments
Content-Type: application/json

Body:
{
  "patientName": "string",
  "email": "string",
  "phone": "string",
  "date": "YYYY-MM-DD",
  "time": "HH:MM",
  "clinicId": "string",
  "clinicName": "string",
  "disease": "string",
  "notes": "string (optional)"
}

Response: Saved appointment object
```

**Get all appointments:**
```
GET /api/appointments

Response: Array of Appointment objects
```

**Cancel appointment:**
```
DELETE /api/appointments/:id

Response: { "success": true }
```

## 🗂️ Project Structure

```
dermavision-ai/
├── src/
│   ├── components/           # React components
│   │   ├── AnalyticsPanel.tsx
│   │   ├── AppointmentsPanel.tsx
│   │   ├── BookingModal.tsx
│   │   ├── ChatBot.tsx
│   │   ├── ClinicCard.tsx
│   │   ├── ClinicsPanel.tsx
│   │   ├── DoctorFinder.tsx
│   │   ├── HistoryView.tsx
│   │   ├── ImageUploader.tsx
│   │   ├── PredictionResult.tsx
│   │   ├── SettingsPanel.tsx
│   │   └── ThemeSwitcher.tsx
│   ├── data/
│   │   └── clinics.ts       # Clinic data
│   ├── hooks/
│   │   └── useSettings.ts   # Settings management
│   ├── lib/
│   │   ├── pdfGenerator.ts  # PDF generation
│   │   └── utils.ts         # Utility functions
│   ├── App.tsx              # Main application
│   ├── index.css            # Global styles
│   ├── main.tsx             # Entry point
│   └── types.ts             # TypeScript types
├── public/
│   └── uploads/             # Uploaded images
├── server.ts                # Express server
├── database.db              # SQLite database
├── .env                     # Environment variables
├── .env.example             # Environment template
├── package.json             # Dependencies
├── tsconfig.json            # TypeScript config
└── vite.config.ts           # Vite config
```

## 🎯 Data Models

### PredictionResult
```typescript
interface PredictionResult {
  id?: number;
  disease: string;
  confidence: number;
  description: string;
  causes: string;
  effects: string;
  symptoms: string;
  prevention: string;
  medicines: string;
  treatment: string;
  image_url: string;
  timestamp?: string;
  probabilities?: { [key: string]: number };
  healthScore?: number;
}
```

### Appointment
```typescript
interface Appointment {
  id?: number;
  patientName: string;
  email: string;
  phone: string;
  date: string;
  time: string;
  clinicId: string;
  clinicName: string;
  disease: string;
  notes?: string;
  status: 'confirmed' | 'cancelled';
  createdAt?: string;
}
```

### AppSettings
```typescript
interface AppSettings {
  theme: 'dark' | 'neon' | 'light';
  wallpaper: 'cyberpunk' | 'scanner' | 'medical' | 'gradient' | 'galaxy';
  voiceEnabled: boolean;
  animationsEnabled: boolean;
  language: 'en' | 'kn';
  locationEnabled: boolean;
  doctorSuggestionsEnabled: boolean;
  chartAnimationsEnabled: boolean;
}
```

## ⚙️ Configuration

### Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `GROQ_API_KEY` | Groq API key for AI models | ✅ Yes |

### Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build |
| `npm run clean` | Remove dist folder |
| `npm run lint` | TypeScript type checking |
| `npm start` | Start production server |

## 🗄️ Database Schema

### History Table
```sql
CREATE TABLE history (
  id INTEGER PRIMARY KEY AUTOINCREMENT,
  disease TEXT,
  confidence REAL,
  description TEXT,
  causes TEXT,
  effects TEXT,
  symptoms TEXT,
  prevention TEXT,
  medicines TEXT,
  treatment TEXT,
  timestamp DATETIME DEFAULT CURRENT_TIMESTAMP,
  image_url TEXT,
  probabilities TEXT
);
```

### Appointments Table
```sql
CREATE TABLE appointments (
  id INTEGER PRIMARY KEY AUTOINCREMENT,
  patientName TEXT NOT NULL,
  email TEXT,
  phone TEXT,
  date TEXT NOT NULL,
  time TEXT NOT NULL,
  clinicId TEXT NOT NULL,
  clinicName TEXT NOT NULL,
  disease TEXT,
  notes TEXT,
  status TEXT DEFAULT 'confirmed',
  createdAt DATETIME DEFAULT CURRENT_TIMESTAMP
);
```

## 🎨 User Interface

### Navigation Tabs
- **Dashboard**: Main interface for image upload and analysis
- **History**: View past analyses and predictions
- **Analysis**: Detailed analytics and charts
- **Clinics**: Browse clinics and manage appointments
- **Settings**: Configure app preferences

### Key UI Components
- **ImageUploader**: Drag-and-drop or click-to-upload interface
- **PredictionResultCard**: Displays diagnosis with full details
- **ChatBot**: Contextual AI assistant
- **AnalyticsPanel**: Interactive charts and metrics
- **ClinicsPanel**: Clinic directory with booking
- **ThemeSwitcher**: Visual theme customization

## 🔒 Privacy & Security

- **Local Storage**: All data stored locally in SQLite database
- **Temporary Files**: Uploaded images are processed and cleaned up
- **No Cloud Storage**: Images are not permanently stored on external servers
- **API Key Security**: Groq API key stored in environment variables only

## ⚠️ Medical Disclaimer

**IMPORTANT**: This application is designed for **educational and diagnostic assistance purposes only**. 

- The AI analysis should **NOT** replace professional medical diagnosis
- Always consult with a qualified dermatologist or healthcare provider
- Results are based on AI predictions and may not be 100% accurate
- Use this tool as a preliminary screening aid, not a definitive diagnosis

## 🛠️ Troubleshooting

### Common Issues

**1. Groq API Key Error**
```
❌ GROQ_API_KEY is missing from .env
```
**Solution**: Create a `.env` file with your valid Groq API key.

**2. Analysis Failed**
- Check your internet connection
- Verify Groq API key is valid and has credits
- Check browser console and server logs for details

**3. Images Not Uploading**
- Ensure file is a valid image format (JPG, PNG, etc.)
- Check file size limits
- Verify `public/uploads` directory exists and is writable

**4. Database Errors**
- Delete `database.db` to reset (will lose all history)
- Check file permissions

### Debug Mode

Enable detailed logging:
```bash
# Check server health
curl http://localhost:3000/api/health

# View console logs in browser developer tools
# Check server terminal for backend logs
```

## 📈 Performance Optimization

- **Image Compression**: Optimize images before upload
- **Database Indexing**: Automatic indexing on timestamps
- **Caching**: Browser caching for static assets
- **Lazy Loading**: Components loaded on demand
- **Production Build**: Use `npm run build` for optimized assets

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Groq**: For providing fast AI inference
- **Meta**: For Llama models
- **React Community**: For excellent documentation
- **Medical Professionals**: For domain expertise

## 📞 Support

For issues, questions, or feedback:
- 🐛 **Bug Reports**: Open an issue on GitHub
- 💡 **Feature Requests**: Open an issue with "enhancement" label
- 📧 **General Questions**: Contact the development team

## 🔮 Future Enhancements

- [ ] Real-time video analysis
- [ ] Multi-language support expansion
- [ ] Integration with hospital management systems
- [ ] Mobile application (React Native)
- [ ] Advanced analytics with machine learning
- [ ] Telemedicine consultation features
- [ ] Skin condition progression tracking
- [ ] Community forum for dermatology discussions

---

**Built with ❤️ for better dermatological healthcare**

*DermaVision AI - Neural Engine v4.0.2*
