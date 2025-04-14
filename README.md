# **AI Video Editor**

**AI Video Editor** is a powerful AI-enhanced video editing platform designed to automate time-consuming post-production tasks such as **speech-to-text transcription**, **scene segmentation**, **activity detection**, and **smart editing**. It integrates traditional editing with advanced machine learning models to help users create professional-quality videos with minimal effort.

The system features a modern **React + Material UI frontend** and a robust **FastAPI backend**, leveraging tools like **OpenCV**, **FFmpeg**, **MoviePy**, and **OpenAI's Whisper** for seamless AI-powered video processing.

---

## **Dataset**

The dataset used for training and testing various AI models was compiled from **multiple video sources**:

- Public video repositories
- Online platforms
- Self-curated content collections

These videos were labeled for tasks like **scene transitions**, **human activity recognition**, and **speech transcription**, ensuring a diverse and realistic training base.

---

## **Key Features**

| Category | Description |
| --- | --- |
| **Speech-to-Text** | Converts spoken words in videos into text using **OpenAI Whisper**, generating time-aligned subtitles automatically. |
| **Scene Recognition** | Detects scene transitions using OpenCV and visual cues like color histograms and frame differences. |
| **Activity Detection** | Recognizes key actions (walking, speaking, turning) with pretrained CNNs to highlight important moments. |
| **Smart Editing** | Trimming, merging, stabilization, and subtitle overlay with MoviePy and FFmpeg. |
| **User Interface** | Web interface to upload videos, select AI features, preview results, and download the edited output. |

---

## **Project Structure**

```
kotlin
CopyEdit
AI-Video-Editor/
│
├── backend/ (FastAPI)
│   ├── models/ (AI Modules)
│   ├── routes/ (API Endpoints)
│   ├── utils/ (Helpers)
│   ├── data/ (uploads/ and processed_videos/)
│   ├── app.py, config.py, requirements.txt
│
├── frontend/ (React + Material UI)
│   ├── src/ (Pages, Components, Config)
│   ├── public/
│   ├── package.json, .env
│
├── README.md

```

---

## **Technologies Used**

| Component | Technologies |
| --- | --- |
| Frontend | React.js, Material UI, Axios |
| Backend | FastAPI (Python), Pydantic |
| Video Editing | MoviePy, FFmpeg |
| AI Modules | OpenCV, Whisper, CNNs |
| Storage | Local (uploads/processed), Cloud-Ready |
| Deployment | Docker support for backend and frontend |

---

## **Installation**

Install dependencies:

```bash
bash
CopyEdit
pip install -r backend/requirements.txt
cd frontend
npm install

```

Run the application:

```bash
bash
CopyEdit
# Start backend
cd backend
uvicorn app:app --reload

# Start frontend
cd ../frontend
npm start

```

---

## **How to Use**

1. **Visit**: [http://localhost:3000](http://localhost:3000/)
2. **Upload** a video file.
3. **Select AI options** like:
    - Speech-to-text
    - Scene recognition
    - Activity detection
4. **Preview** the edited video.
5. **Download** the final output with embedded subtitles and enhancements.

---

## **Use Cases**

- **Educational Content Creation**
- **Social Media Reels & Shorts**
- **Corporate Training Videos**
- **News Editing & Journalism**
- **YouTube & Vlog Automation**

---

## **Performance Highlights**

| Task | Accuracy / Metric |
| --- | --- |
| Scene Recognition | 94% accuracy |
| Speech-to-Text | 90%+ transcription accuracy (WER ≤ 10%) |
| Activity Detection | 86% average accuracy |
| Subtitle Precision | F1-score ~0.90 |

Average editing time was **reduced by 60%**, making the system ideal for fast-paced content generation.

---

## **Contributors**

- [Adarsh Nashine](https://github.com/adarsh-n2003)
- [Anuj Tirole](https://github.com/anujtirole)
- [Prabal Singh](https://github.com/Prabalsing)
- [Surendra Singh Koranga](https://github.com/Surendrasingh6289)

**Institution**: Prestige Institute of Engineering Management and Research, Indore

**Guide**: Dr. Naveen R. Shahi

---

## **Future Scope**

- Real-time video editing and streaming support
- Multilingual subtitle generation
- Gesture-based AI editing
- Cloud collaboration and storage (AWS, Firebase)
- Personalized editing based on user behavior

---

## **License**

This project is licensed under the **MIT License**.
