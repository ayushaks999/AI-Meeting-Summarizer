# 🎤 AI Meeting Summarizer

> A powerful desktop application that records, transcribes, summarizes, and generates actionable items from meetings using advanced AI technology.

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![Python](https://img.shields.io/badge/python-3.8+-green.svg)
![Node](https://img.shields.io/badge/node-18+-green.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

---

## ✨ Features

### Core Capabilities

* 🎙️ **Local Audio Capture** - Record meetings directly from your microphone
* ⚡ **Real-Time Transcription** - See transcription appear every 10 seconds while recording
* 🤖 **AI-Powered Summarization** - Get detailed, comprehensive meeting summaries
* 📋 **Action Item Extraction** - Automatically identify tasks, assignments, and deadlines
* 🎯 **Smart Task Lists** - Auto-generated task lists with priorities and assignees
* 🔔 **Desktop Notifications** - Real-time notifications for all major events

### Integrations

* 📅 **Google Calendar Sync** - Export action items as calendar events
* 📝 **Notion Export** - Send meeting notes to Notion pages
* 🎯 **Jira Task Sync** - Create Jira tasks from action items
* 🌐 **Language Translation** - Translate meetings to 12+ languages

### Additional Features

* ✏️ **Meeting Title Editing** - Edit and customize meeting titles
* 🎵 **Audio Playback** - Listen to recorded audio from meeting details
* 🔍 **Advanced Search & Filters** - Find meetings by date, title, or action item status
* 👥 **Participant Tracking** - Track meeting attendees
* 💾 **Local Storage** - All data stored locally in SQLite database

---

## 🎬 Demo

```
screenshots/
├── main-view.png
├── recording-view.png
├── live-transcription.png
└── meeting-details.png
```

---

## 🛠️ Tech Stack

### Desktop Framework

* **Electron** - Cross-platform desktop application

### Backend

* **Python 3.8+** - Core backend runtime
* **Flask** - Web framework
* **Flask-SocketIO** - Real-time communication
* **SQLAlchemy** - Database ORM
* **SQLite** - Local database

### AI Services

* **Deepgram API** - Speech-to-text transcription
* **Euron.one API** - GPT-4.1 mini for summarization and action item extraction
* **Deep Translator** - Multi-language translation

### Frontend

* **HTML/CSS/JavaScript** - UI implementation
* **Axios** - HTTP client
* **Socket.IO Client** - Real-time updates

---

## 📦 Installation

### Prerequisites

* **Python 3.8+**
* **Node.js 18+**
* **Git**

### Step 1: Clone Repository

```bash
git clone https://github.com/ayushaks999/AI_Meeting_Summarizer.git
cd AI_Meeting_Summarizer
```

### Step 2: Install Python Dependencies

```bash
python -m venv venv

# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

pip install -r requirements.txt
```

### Step 3: Install Node Dependencies

```bash
npm install
```

### Step 4: Configure Environment Variables

Create a `.env` file in the root directory:

```env
TRANSCRIPTION_MODEL=deepgram
DEEPGRAM_API_KEY=your_deepgram_api_key_here

USE_EURON_API=true
EURON_API_KEY=your_euron_api_key_here
EURON_API_BASE=https://api.euron.one/v1
EURON_MODEL=gpt-4.1-mini

DEBUG=False
DATABASE_PATH=data/meetings.db
```

---

## 🚀 Usage

### Start the Application

```bash
npm start
```

This command will:

1. Start the Python backend on `http://127.0.0.1:5000`
2. Launch the Electron desktop app

---

## 🧪 Development

```bash
# Backend
python backend/app.py

# Frontend (separate terminal)
npm run start:electron
```

---

## 📝 Features Roadmap

* [ ] Speaker diarization
* [ ] Meeting templates
* [ ] Export to PDF
* [ ] Meeting analytics dashboard
* [ ] Cloud sync

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License.

---

## 📧 Support

For issues or suggestions:

* Open an issue on GitHub: [https://github.com/ayushaks999/AI_Meeting_Summarizer/issues](https://github.com/ayushaks999/AI_Meeting_Summarizer/issues)

---

## 🌟 Show Your Support

If this project helped you, please give it a ⭐!

---

**Made with ❤️ by Ayush Kumar Shaw**
