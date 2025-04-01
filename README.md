# JobRefMe

<p align="center">
  <img src="public/logo.png" alt="JobRefMe Logo" width="128" height="128">
</p>

<p align="center">
  <strong>AI-powered job referral message generator for maximizing your networking opportunities</strong>
</p>

<p align="center">
  <a href="https://jobrefme.fly.dev" target="_blank">Visit Live Site</a> •
  <a href="#installation">Installation Guide</a> •
  <a href="#features">Features</a> •
  <a href="#documentation">Documentation</a>
</p>

## Overview

JobRefMe is an intelligent solution that helps job seekers craft personalized referral request messages based on job postings. Leveraging Google's Gemini AI, it analyzes job descriptions and generates tailored messages that highlight relevant skills and qualifications, making it easier to request referrals from your professional network.

## 🚀 Project Components

JobRefMe consists of two main components:

### 1. [JobRefMe Chrome Extension](https://github.com/Prathmesh-Dhatrak/jobrefme-extension)

A browser extension that integrates with job boards to generate personalized referral requests directly while browsing.

**Repository:** [github.com/Prathmesh-Dhatrak/jobrefme-extension](https://github.com/Prathmesh-Dhatrak/jobrefme-extension)

- **Features**: Generate referrals from HireJobs.in job postings or from any selected job description text
- **Technologies**: React, TypeScript, Tailwind CSS, Chrome Extension Manifest V3

### 2. [JobRefMe Backend](https://github.com/Prathmesh-Dhatrak/jobrefme-backend)

A Node.js backend service that powers the extension with job data extraction and AI-powered message generation.

**Repository:** [github.com/Prathmesh-Dhatrak/jobrefme-backend](https://github.com/Prathmesh-Dhatrak/jobrefme-backend)

- **Features**: Job data extraction, AI message generation, user authentication, template management
- **Technologies**: Node.js, Express, TypeScript, MongoDB, Google OAuth, Gemini AI

## ✨ Features

- **Two Referral Generation Methods**:
  - **Website Integration**: Automatically detect job details from supported job boards
  - **Universal Content Selection**: Generate referrals from job descriptions on any website
  
- **AI-Powered Generation**: Uses Google's Gemini AI to create tailored referral messages
- **Relevant Skills Highlighting**: Identifies and emphasizes skills from the job posting
- **One-Click Copy**: Easily copy the generated message with one click
- **Google Account Integration**: Save your preferences and templates
- **Custom Templates**: Create and manage your own referral message templates
- **API Key Management**: Securely store and manage your Gemini API key

## 🛠️ Installation

As the extension is not yet published to the Chrome Web Store, you'll need to install it in developer mode.

### Installing the Chrome Extension

1. **Download the Extension**:
   - Go to the [latest release page](https://github.com/Prathmesh-Dhatrak/jobrefme-extension/releases/latest)
   - Download the `jobrefme-extension.zip` file
   - Extract the zip file to a location on your computer

2. **Load in Chrome**:
   - Open Chrome and navigate to `chrome://extensions/`
   - Enable "Developer mode" in the top-right corner
   - Click "Load unpacked" and select the extracted folder

3. **Initial Setup**:
   - After installation, a welcome page will open automatically
   - Enter your Google Gemini API key ([Get one here](https://ai.google.dev/))
   - Click "Save API Key" to store it securely

### Getting a Gemini API Key

1. Visit [Google AI Studio](https://ai.google.dev/)
2. Sign in with your Google account
3. Go to "API keys" section
4. Click "Create API Key"
5. Copy the generated key and use it in the extension

## 🧑‍💻 Development Setup

If you want to contribute or modify the extension:

### Chrome Extension

```bash
# Clone the repository
git clone https://github.com/Prathmesh-Dhatrak/jobrefme-extension.git
cd jobrefme-extension

# Install dependencies
yarn install

# Start development server
yarn dev

# Build for production
yarn build
```

### Backend Service

```bash
# Clone the repository
git clone https://github.com/Prathmesh-Dhatrak/jobrefme-backend.git
cd jobrefme-backend

# Install dependencies
npm install

# Set up environment variables
cp .env.sample .env
# Edit .env with your configuration

# Start development server
npm run dev

# Build for production
npm run build
```

## 📖 Documentation

- [Extension Documentation](https://github.com/Prathmesh-Dhatrak/jobrefme-extension#readme)
- [Backend API Documentation](https://github.com/Prathmesh-Dhatrak/jobrefme-backend#-api-endpoints)
- [User Guide](https://jobrefme.fly.dev/docs)

## 🔒 Privacy

- Your Gemini API key is stored securely in your browser's local storage
- No personal data is collected or sent to our servers
- API requests are made directly from the extension to Google's Gemini API using your key

## 👨‍💻 Author

**Prathmesh Dhatrak** - [GitHub](https://github.com/Prathmesh-Dhatrak) | [LinkedIn](https://linkedin.com/in/prathmesh-dhatrak) | [Website](https://prathmeshdhatrak.com)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
