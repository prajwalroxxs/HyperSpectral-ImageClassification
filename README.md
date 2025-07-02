# 🧠 Multi-Modal Fake News Detection System

A comprehensive deep learning research project combining **Natural Language Processing (NLP)** and **Computer Vision (CV)** to detect fake news content. This system analyzes both **text and images** to deliver robust binary classification, confidence scores, and explainable reports.

---

## 🚀 Features

- 🧩 **Multi-Modal Analysis**: Fusion of text and image-based predictions  
- 📄 **Text Classification**:  
  - BERT-based semantic understanding  
  - Feature-based linguistic analysis  
- 🖼️ **Image Analysis**:  
  - Error Level Analysis (ELA) for image tampering  
  - OCR-based text extraction and suspicious pattern detection  
- 📊 **Comprehensive Output**:  
  - Binary output: `Fake` / `Real`  
  - Confidence scores per modality  
  - Risk indicators and recommendations  
- 📁 **Research-Oriented**:  
  - Jupyter notebooks  
  - API endpoints for real-time usage  
  - Visual analytics and performance metrics  

---

## 🧱 Architecture

ml_components/
├── utils/
│ └── data_utils.py
├── preprocessing/
│ ├── text_processor.py
│ └── image_processor.py
├── models/
│ ├── nlp/text_classifier.py
│ ├── computer_vision/image_classifier.py
│ └── fusion/multimodal_classifier.py
└── notebooks/
└── fake_news_detection_research.ipynb

markdown
Copy
Edit

---

## ⚙️ Technology Stack

- **Backend**: FastAPI, Python  
- **Machine Learning**: TensorFlow, scikit-learn, transformers  
- **NLP**: BERT, NLTK, TextBlob  
- **Computer Vision**: OpenCV, PIL, pytesseract  
- **Data Handling**: pandas, numpy  
- **Visualization**: matplotlib, seaborn, plotly  
- **Database**: MongoDB  

---

## 📊 Model Components

### 1. 📝 NLP
- **BERT Classifier**
- **Feature-Based Classifier**
  - Sentiment, punctuation, readability, and linguistic complexity

### 2. 🖼️ Computer Vision
- **Image Manipulation Detection**
  - Error Level Analysis (ELA) and compression artifact detection
- **OCR Text Analysis**
  - Text extraction and scoring based on OCR quality and suspicious patterns

### 3. 🔄 Multi-Modal Fusion
- Weighted Average
- Majority Voting
- Meta-learned classifier for optimal fusion

---

## 📡 API Endpoints

| Method | Endpoint                     | Description                      |
|--------|------------------------------|----------------------------------|
| POST   | `/api/analyze`               | Multi-modal analysis             |
| POST   | `/api/analyze/text-only`     | Text-only classification         |
| POST   | `/api/analyze/image-only`    | Image-only classification        |
| GET    | `/api/system/status`         | System health check              |
| POST   | `/api/system/initialize`     | Initialize/reload ML models      |
| GET    | `/api/analyze/history`       | Retrieve analysis history        |
