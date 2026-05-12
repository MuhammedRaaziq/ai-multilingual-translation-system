# 🎓 AI-Based Multilingual Lecture Translation System

## 📌 Overview
This project is an AI-based multilingual lecture translation system designed to assist first-year university students in understanding lectures in real time. It captures live lecturer speech, processes it and translates it into multiple South African languages (isiZulu, isiXhosa and Afrikaans), improving accessibility and equitability in higher education.

---

## 🚀 Features

### 👨‍🏫 Lecturer Panel
- Live speech-to-text capture using browser microphone
- Real-time broadcasting of lecture content
- Start/stop microphone control
- Live preview of spoken text

### 🎓 Student Panel
- Real-time lecture text display
- Instant multilingual translation
- Language selection (isiZulu, isiXhosa, Afrikaans)
- Optional voice output (text-to-speech)
- Dark mode support
- Live system status indicator
- Adjustable volume and reading speed

---

## 🧠 System Architecture

The system follows a real-time event-driven architecture:

1. Lecturer speaks into microphone  
2. Browser Speech Recognition API converts speech to text  
3. Text is sent to the Flask backend using Socket.IO  
4. Backend processes translation using GoogleTranslator (deep-translator)  
5. Translated output is sent back to connected students  
6. Student interface displays translated text and optionally reads it aloud using speech synthesis  

---

## 🛠️ Tech Stack

### Frontend
- HTML5
- CSS3 (Custom UI + Dark Mode)
- JavaScript (ES6)
- Socket.IO (Real-time communication)
- Web Speech API (Speech recognition & synthesis)

### Backend
- Python 3
- Flask
- Flask-SocketIO
- deep-translator (Google Translate wrapper)

---

## 📂 Project Structure

ai-translation-system/  
│  
├── backend.py  
├── requirements.txt  
├── README.md  
│  
├── templates/  
│   ├── lecturer.html  
│   └── student.html  

---

## ⚙️ Installation & Setup

1. Clone the repository  
git clone https://github.com/your-username/ai-translation-system.git  

2. Navigate into project folder  
cd ai-translation-system  

3. Install dependencies  
pip install -r requirements.txt  

4. Run backend server  
python backend.py  

5. Open in browser  

Lecturer Panel:  
http://127.0.0.1:5000  

Student Panel:  
http://127.0.0.1:5000/student  

---

## 🌍 Supported Languages
- isiZulu (zu)  
- isiXhosa (xh)  
- Afrikaans (af)  

---

## 💡 Key Innovation
- Real-time lecture translation system using web technologies  
- Supports multilingual education in South African universities  
- Reduces language barriers for first-year students  
- Lightweight browser-based system (no installation required for users)  

---

## ⚠️ Limitations
- Requires stable internet connection  
- Depends on browser speech recognition accuracy  
- Translation quality depends on GoogleTranslator service  
- Works best in Chrome browser  

---

## 🔮 Future Improvements
- Offline AI translation model (NLP-based)  
- User authentication system (students/lecturers)  
- Save lecture transcripts to database  
- Add more African languages  
- Deploy system online using cloud hosting (AWS / Render / Vercel)  

---
