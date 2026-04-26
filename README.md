
# 🔐 EthicalDRM  
### Track Piracy Without Punishing Users

> EthicalDRM is a forensic Digital Rights Management (DRM) system that focuses on **traceability, accountability, and intelligent detection**—instead of restricting users.

🎬 **Live Demo:**  
👉 https://drive.google.com/file/d/1Ha8rNBAHfYhCZHMVyPT7oFB0N48IloDP/view?usp=sharing

---

## 🚀 Overview

Traditional DRM systems restrict access and often degrade user experience.  
EthicalDRM takes a different approach:

> **We don’t try to stop piracy — we make it accountable and traceable.**

The system embeds invisible identity signals into content and tracks how and where it gets redistributed.

---

## 🏆 Hackathon Context

- ⏱ Built in **48 hours**
- 👥 Team Project
- 🎯 Focus: Real-world, practical DRM solution
- 💡 Goal: Balance **user experience + security**

---

## 📸 Demo Preview

🎬 **Project Demo Video:**  
[▶️ Watch EthicalDRM in Action](https://drive.google.com/file/d/1Ha8rNBAHfYhCZHMVyPT7oFB0N48IloDP/view?usp=sharing)

📌 Demonstrates:
- Watermark embedding  
- Leak simulation  
- Detection pipeline  
- Source tracing  
- AI-generated DMCA report  

---

**Pipeline:**
```

Protect → Leak → Detect → Trace → Respond

````

**Workflow:**
1. Upload content  
2. Watermark per user  
3. Simulate or detect leak  
4. Scan file or URL  
5. Identify source  
6. Generate DMCA report  

---

## ❗ Problem Statement

Digital creators face major challenges:

- No control once content is shared  
- Traditional DRM frustrates real users  
- No way to identify *who leaked content*  
- No visibility into *where content spreads*  

---

## ✅ Our Solution

EthicalDRM shifts the focus from **restriction → attribution**

- Embed invisible watermarks per user  
- Detect leaks even after edits/compression  
- Identify source with confidence score  
- Track distribution across public platforms  
- Generate automated legal response  

---

## ⚡ Key Features

| Feature | Description |
|--------|------------|
| 🎥 Video Watermarking | Frame-by-frame watermarking using OpenCV |
| 🖼️ Image Watermarking | Pixel-level watermark embedding |
| 🧠 Perceptual Hashing | Detects modified/compressed media |
| 🔍 Leak Detection | Identifies source with confidence score |
| 🌐 Web Crawler | Scans public sites for leaked content |
| 🤖 AI DMCA Generator | Auto-generates legal reports (Gemini) |
| 🔗 Public Link Scanning | Extracts and verifies media URLs |

---

## 🏗️ System Architecture

### 1. UI Layer
- Streamlit (`app.py`)

### 2. Core Processing
- Watermarking (video + image)  
- Perceptual hashing  
- Leak detection  
- Web crawling  

### 3. AI Layer
- DMCA report generation  

### 4. Storage
- Original media  
- Watermarked content  
- Simulated leaks  

---

## 🔄 How It Works

### 🔐 Media Protection
- Upload content  
- Apply user-specific watermark  
- Generate perceptual hash  

### 🔍 Leak Detection
- Scan leaked file or URL  
- Compare hashes  
- Identify:
  - User ID  
  - Confidence score  

### 📄 Legal Response
- Generate DMCA-style report  
- AI-powered + fallback template  

---

## 🌐 Crawler System

- Crawls public webpages  
- Extracts media links (`.mp4`, `.jpg`, `.png`)  
- Downloads limited files  
- Runs detection pipeline  

### Example Output:
```json
{
  "platform": "Web",
  "url": "https://example.com/video",
  "user": "user_123",
  "confidence": 87.5
}
````

---

## 🤖 AI Integration

* Powered by **Google Gemini API**
* Generates structured DMCA reports
* Includes fallback system for reliability

---

## 🛠️ Tech Stack

* **Frontend/UI:** Streamlit
* **Backend:** Python
* **Media Processing:** OpenCV, Pillow
* **Hashing:** ImageHash
* **Web Crawling:** Requests, BeautifulSoup
* **AI:** Google Gemini API

---

## 📁 Project Structure

```
ethical_drm/
├── app.py
├── README.md
├── requirements.txt
├── core/
│   ├── watermark.py
│   ├── image_watermark.py
│   ├── hashing.py
│   ├── detector.py
│   ├── crawler.py
│   └── utils.py
├── ai/
│   └── dmca_generator.py
├── database/
│   └── db.py
└── storage/
    ├── original_videos/
    ├── watermarked_videos/
    └── simulated_leaks/
```

---

## ⚙️ Installation

```bash
git clone https://github.com/your-username/EthicalDRM.git
cd EthicalDRM

python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate

pip install -r requirements.txt
```

---

## 🔑 Environment Setup (Optional)

```bash
export GEMINI_API_KEY="your_api_key"
```

---

## ▶️ Usage

```bash
streamlit run app.py
```

---

## 🧪 Demo Flow

1. Upload `original.mp4`
2. Watermark for `user_007`
3. Simulate leak
4. Scan URL/file
5. View:

   * Source user
   * Confidence score
6. Generate DMCA report

---

## ⚠️ Limitations

* Works only on publicly accessible content
* Telegram crawler is conceptual
* Confidence scoring is heuristic-based

---

## 🔮 Future Scope

* Telegram & dark web crawling
* ML-based detection improvements
* Real-time monitoring dashboard
* SaaS deployment
* Blockchain-based ownership tracking

---

## 🧠 Core Idea

> **Accountability over control.**

* No harsh restrictions
* No degraded user experience
* Focus on traceability

---

## 🤝 Contributing

```bash
git checkout -b feature/your-feature
git commit -m "feat: add feature"
git push origin feature/your-feature
```

---

## 👨‍💻 Contributors

* Your Name
* Team Members

---

## 📄 License

Choose before production:

* MIT License
* Apache 2.0

---

## ⭐ Support

If you found this project interesting, consider giving it a ⭐ on GitHub!

```

