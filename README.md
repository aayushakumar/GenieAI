
# 🧞 GenieAI – The AI-Powered Scam & Spam Forensics Assistant

Genie is a privacy-first, multimodal AI assistant that helps you analyze messages (emails, texts, DMs, or screenshots) to detect:

- 🧠 Spam & Phishing
- 🤖 AI-Generated Text (LLM-crafted scams)
- 🧑‍💻 Suspicious Senders & Metadata
- 🖼️ Screenshot-based scams via OCR
- 🔒 Full Offline Mode support
- 🧩 Chrome Plugin integration for Gmail, Outlook, and more

---

## 🚀 Key Features

| Feature | Description |
|--------|-------------|
| 🔍 Spam & Scam Detection | Classify emails/texts as spam, phishing, or legit |
| 🤖 AI-Written Message Detection | Identify LLM-generated content via stylometry or detectors |
| 🖼️ Screenshot OCR + Analysis | Upload screenshots; Genie extracts text and analyzes it |
| 🌐 Sender Metadata Extraction | Domain reputation, spoofed sender detection, language fingerprinting |
| 🧪 Forensics Explanation | Why was something flagged? See threat breakdowns with reasoning |
| 🧱 Offline Mode | Fully local version with all models run on-device |
| 🧩 Chrome Plugin | Inline message flagging in Gmail, Outlook, etc. |

---

## 🧠 How It Works

1. **Input Layer**: Accepts raw text or screenshots  
2. **OCR Engine**: Converts screenshots to analyzable text  
3. **Model Layer**:
   - Spam/Phishing Classifier (fine-tuned BERT/RoBERTa)
   - AI-Text Detector (GPTZero-style, stylometry, classifiers)
4. **LLM Reasoning (Optional)**: Uses ReAct agent to explain decisions  
5. **Output**: Displays threat flags, scores, and generates a forensics PDF if needed  
6. **Browser Extension**: Real-time Gmail message scanning + highlighting

---

## 🧰 Tech Stack

- `Python`, `FastAPI`, `Gradio`, or `Streamlit` for the UI/backend
- `OCR`: [Tesseract](https://github.com/tesseract-ocr/tesseract), [EasyOCR](https://github.com/JaidedAI/EasyOCR)
- `ML Models`: BERT, RoBERTa, GPT2-detector, etc.
- `Frontend`: Electron for desktop app OR Chrome Extension
- Optional APIs: VirusTotal, URLScan, PhishTank

---

## 🛠️ Setup Instructions (MVP)

```bash
# Clone the repo
git clone https://github.com/yourusername/genie-ai
cd genie-ai

# Install dependencies
pip install -r requirements.txt

# Start the app
python app.py  # Or streamlit run app.py
```

---

## ✨ Use Cases

- Security-conscious individuals
- Journalists & fact-checkers
- Enterprise threat triage tools
- Governments or offline-sensitive organizations

---

## 📦 Roadmap

### Phase 1 – MVP (Text + Screenshot)
- [ ] Spam/Phishing Detection
- [ ] Screenshot OCR pipeline
- [ ] AI-written message detection

### Phase 2 – UX + Deployments
- [ ] Chrome Extension for Gmail
- [ ] Offline desktop app (Electron or local server)
- [ ] Forensics report generation (PDF/HTML)

### Phase 3 – Enhancements
- [ ] LLM ReAct explanation
- [ ] Real-time threat intelligence (VirusTotal, etc.)
- [ ] Continuous feedback learning loop

---

## 🔒 Privacy & Security

Genie can run **fully offline**. No data leaves your device unless you explicitly opt in to use cloud APIs. Ideal for high-trust and air-gapped environments.

---

## 📄 License

MIT License

---
