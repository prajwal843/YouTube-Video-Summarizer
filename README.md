# YouTube-Video-Summarizer

# 📺 YouTube Video Summarizer Chrome Extension

This Chrome extension helps users **quickly understand the content of YouTube videos** by providing **concise summaries** using AI-powered NLP models. It extracts the video transcript and generates a short summary, saving users time and improving content accessibility.

---

## 🚀 Features

- 🔍 Automatically fetches the transcript of YouTube videos
- 🧠 Summarizes long transcripts using Hugging Face Transformers
- ⚡ Fast, lightweight, and easy-to-use Chrome extension
- 🌐 Clean HTML & JavaScript frontend
- 🐍 Flask-powered backend API

---

## 🛠️ Technologies Used

- **Python** (Backend)
- **Flask** – for serving the summarization API
- **YouTube Transcript API** – to extract subtitles from videos
- **Hugging Face Transformers** – for state-of-the-art summarization
- **HTML, CSS, JavaScript** – for Chrome extension frontend

---

## 📦 Project Structure

youtube-summarizer-extension/
│
├── backend/
│ ├── app.py # Flask API for transcript and summary
│ ├── summarizer.py # Hugging Face transformer summarizer logic
│ └── requirements.txt # Python dependencies
│
├── extension/
│ ├── popup.html # Extension UI
│ ├── popup.js # JS logic to interact with backend
│ └── manifest.json # Chrome extension config
│
└── README.md # Project documentation

yaml
Copy
Edit

---

## 💡 How It Works

1. **User opens a YouTube video**
2. **Chrome extension button is clicked**
3. **Extension sends video URL to Flask API**
4. **API uses YouTube Transcript API to get transcript**
5. **Transcript is summarized using Hugging Face model**
6. **Summary is returned and displayed in the popup UI**

---

## 🧪 Setup Instructions

### Backend (Flask API)

```bash
cd backend
pip install -r requirements.txt
python app.py
Frontend (Chrome Extension)
Open Chrome and go to chrome://extensions/

Enable Developer Mode

Click Load unpacked

Select the extension/ folder

The extension will appear in your browser toolbar

⚠️ Make sure the Flask server is running for the extension to work.

🧠 Future Improvements
Add support for videos without transcripts using speech-to-text

Improve UI/UX for better readability

Option to select summary length (short/medium/detailed)
