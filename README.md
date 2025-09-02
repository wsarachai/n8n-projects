# n8n Business Automation Project

A comprehensive collection of n8n automation workflows designed for Thai businesses, featuring AI-powered document processing, customer service automation, content creation, and business intelligence systems.

## 📋 Table of Contents

- [Overview](#overview)
- [Main Use Cases](#main-use-cases)
- [Bonus Features](#bonus-features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Contributing](#contributing)

## 🌟 Overview

This project contains 10 main use cases and 2 bonus features, each demonstrating advanced integration of various AI services (OpenAI, Mistral, Gemini) with business tools (Google Workspace, LINE, email systems) to create end-to-end business process automation.

## 🎯 Main Use Cases

### 📝 USEC01-Google Form - Fortune Telling Automation

**Purpose**: Automated fortune telling service using Google Forms

**Features**:
- ✅ Collects user data (name, gender, birthdate) via Google Forms
- 🤖 Uses AI to generate personalized fortune predictions
- 📧 Sends results via beautifully formatted HTML emails
- 📊 Tracks customer data in Google Sheets

**Business Use**: Thai fortune telling service ("พ่อหมอออนไลน์") with automated customer engagement

---

### ✅ USEC02-Wait Approve - Content Approval Workflow

**Purpose**: Content creation workflow with human approval system

**Features**:
- ✍️ Creates SEO-optimized blog articles using AI
- 📧 Sends content for human review via email forms
- 🔄 Handles revisions based on feedback
- 📈 Manages content publishing pipeline

**Business Use**: Content marketing automation with quality control

---

### 📄 USEC03-Memo Document - Corporate Memo Automation

**Purpose**: Internal corporate document generation and approval system

**Features**:
- 📝 Form-based memo creation
- 📋 Automated document generation using templates
- 📧 Email distribution to approvers
- 📊 Google Sheets tracking

**Business Use**: Corporate communication and document workflow automation

---

### ⭐ USEC04-Customer Review Analysis - Sentiment Analysis System

**Purpose**: Automated customer review analysis and response generation

**Features**:
- 🔍 Analyzes Thai customer reviews for sentiment
- 📊 Severity rating (1-5) and brand impact assessment
- 💡 Improvement suggestions
- 🤝 Generates appropriate customer responses

**Business Use**: Customer service automation and reputation management

---

### 👁️ USEC05-OCR - Document Processing System

**Purpose**: Optical Character Recognition for financial documents

**Features**:
- 📑 Processes invoices, receipts, and financial documents
- 🤖 Uses Mistral OCR for text extraction
- 🏗️ Extracts structured data (seller info, amounts, VAT, etc.)
- 📊 Stores results in Google Sheets

**Business Use**: Financial document digitization and data entry automation

---

### 📧 USEC06-EMail Classifier - Email Processing System

**Purpose**: Automated email classification and file processing

**Features**:
- 📮 Monitors emails with attachments
- 📁 Creates daily folders in Google Drive
- 🏷️ Classifies finance-related emails
- 📎 Processes attached documents

**Business Use**: Email management and document organization automation

---

### 🎙️ USEC07-TTS And STT - Audio Processing System

**Purpose**: Text-to-Speech and Speech-to-Text conversion

**Features**:
- 🗣️ Converts text to speech using Gemini TTS with various voice styles
- 👂 Converts audio to text using STT
- ☁️ Manages audio files in Google Drive
- 🎚️ Multiple voice style options (30+ voices available)

**Business Use**: Audio content creation and voice interaction automation

---

### 💬 USEC08-Line HelpDesk - LINE Messaging Bot

**Purpose**: Customer support chatbot via LINE messaging platform

**Features**:
- 🔗 LINE webhook integration with signature verification
- 💬 Processes text and image messages
- 🤖 Provides automated customer support responses
- 📱 Mobile-friendly customer service

**Business Use**: Social media customer service automation

---

### 🎯 USEC09-Lead Search - Lead Generation System

**Purpose**: Automated lead generation from various online sources

**Features**:
- 🔍 Searches Facebook, Google, and Maps for potential customers
- 🏢 Extracts business information
- 📍 Organizes leads by location and criteria
- 📊 Configurable search parameters (10-50 results)

**Business Use**: Sales and marketing lead generation automation

---

### 📰 USEC10-Write Content - Multi-Agent Newsletter System

**Purpose**: Automated newsletter creation using multiple AI agents

**Features**:
- ⏰ Scheduled content research and topic planning
- 👥 Multiple specialized AI agents for section writing
- 📝 Content aggregation and final editing
- 🔗 Proper citation management with clickable links
- 📧 Ready-to-send HTML newsletter format

**Business Use**: Content marketing and newsletter automation

---

## 🎁 Bonus Features

### 🤖 BONUS-AI AGENT - Multi-Purpose AI Assistant

**Purpose**: Comprehensive AI assistant with multiple specialized agents

**Components**:
- 📧 **Email Agent** - Email management and sending
- 📅 **Calendar Agent** - Appointment scheduling and management
- 👥 **Contact Agent** - Contact information management
- ✍️ **Content Creator Agent** - Blog post and content creation
- 🌐 **Web Scraping Agent** - Data extraction from websites
- 🖼️ **Image Generation Agent** - AI-powered image creation
- 🧮 **Calculator** - Mathematical computations
- 🧠 **Memory System** - Conversation history management

**Business Use**: All-in-one business automation assistant with conversation memory

---

### 📚 BONUS-RAG - Document Q&A System

**Purpose**: Retrieval-Augmented Generation system using Qdrant vector database

**Features**:
- 📄 Processes various document types (PDF, Word, Google Docs, Images)
- 🔍 Creates vector embeddings for intelligent search
- ❓ Enables document question-answering
- 🗄️ Vector database storage with Qdrant
- 🔗 Integration with multiple document sources

**Business Use**: Knowledge management and document intelligence system

---

## 🛠️ Prerequisites

- **n8n** (self-hosted or cloud)
- **API Keys Required**:
  - OpenAI API
  - Google Workspace APIs (Drive, Sheets, Gmail)
  - LINE Messaging API (for LINE bot)
  - Mistral API (for OCR)
  - OpenRouter API
  - Tavily API (for research)
  - Qdrant Cloud (for RAG system)

## 📦 Installation

1. **Clone or download this repository**
2. **Import workflows into n8n**:
   - Navigate to your n8n instance
   - Go to Workflows → Import from File
   - Select the desired `.json` file from any folder
3. **Configure credentials** for each workflow as needed
4. **Update configuration variables** in the "Set Config" or "Master Config" nodes
5. **Test workflows** before deploying to production

## 🚀 Usage

Each folder contains:
- 📄 **Workflow JSON file** - Import this into n8n
- 📊 **Excel files** - Supporting data and configuration
- 🖼️ **Screenshots** - Visual workflow representations

### Quick Start Guide:

1. Start with simpler workflows like **USEC01-Google Form**
2. Configure your API credentials
3. Test with sample data
4. Gradually move to more complex workflows
5. Use the **BONUS-AI AGENT** as your central automation hub

## 📁 File Structure

```
├── USEC01-Google Form/           # Fortune telling automation
├── USEC02-Wait Approve/          # Content approval workflow  
├── USEC03-Memo Document/         # Corporate memo system
├── USEC04-Customer Review Analysis/ # Sentiment analysis
├── USEC05-OCR/                   # Document OCR processing
├── USEC06-EMail Classifier/      # Email automation
├── USEC07-TTS And STT/          # Audio processing
├── USEC08-Line HelpDesk/        # LINE messaging bot
├── USEC09-Lead Search/          # Lead generation
├── USEC10-Write Content/        # Newsletter automation
├── BONUS-AI AGENT/              # Multi-purpose AI assistant
├── BONUS-RAG/                   # Document Q&A system
└── README.md                    # This file
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Test your workflows thoroughly
4. Submit a pull request with detailed descriptions

## 📝 Notes

- **Language**: Primary language is Thai (ภาษาไทย) for user-facing content
- **Security**: Ensure all API keys and credentials are properly secured
- **Scalability**: Test workflows with your expected data volumes
- **Customization**: Most workflows can be adapted for different business needs

## 📞 Support

For questions or issues:
- Check the n8n community forums
- Review the workflow screenshots for visual guidance
- Test individual nodes before running complete workflows

---

**Created with ❤️ for the n8n automation community**

> This project demonstrates the power of n8n for creating sophisticated business automation workflows using modern AI services and cloud integrations.
