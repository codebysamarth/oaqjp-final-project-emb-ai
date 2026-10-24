# Emotion Detection Application

A web-based AI application that detects human emotions from input text, built as the final project for the Coursera course **Developing AI Applications with Python and Flask** (IBM).

---

## Project Overview

The **Emotion Detection Application** utilizes IBM Watson NLP libraries and Flask to provide real-time emotional analysis on text statements. It evaluates five emotional categories:
- **Anger**
- **Disgust**
- **Fear**
- **Joy**
- **Sadness**

The application also identifies and returns the **dominant emotion** with the highest score.

---

## Project Structure

```text
final_project/
├── EmotionDetection/
│   ├── __init__.py               # Package initialization
│   └── emotion_detection.py      # Core NLP emotion detection logic
├── static/
│   └── mywebscript.js            # Frontend JavaScript for AJAX API calls
├── templates/
│   └── index.html                # Application user interface
├── server.py                     # Flask web server and routing
├── test_emotion_detection.py     # Unit tests for emotion detection
└── README.md                     # Project documentation
```

---

## Key Features

- **Watson NLP Integration**: Connects to the Watson NLP Emotion Predict API to process natural language text.
- **Robust Output Formatting**: Extracts scores for anger, disgust, fear, joy, and sadness, and determines the dominant emotion.
- **Modular Packaging**: Encapsulated within the importable `EmotionDetection` Python package.
- **Comprehensive Unit Testing**: Validates detection accuracy across multiple emotional scenarios using `unittest`.
- **Web Deployment via Flask**: Deployed on `localhost:5000` with clean UI and AJAX handling.
- **Graceful Error Handling**: Detects empty or invalid inputs (HTTP 400) and displays user-friendly error messages (*"Invalid text! Please try again!"*).
- **PEP 8 Compliant**: Verified with `pylint` achieving a perfect **10.00/10** score.

---

## Installation & Running Locally

1. **Clone the repository:**
   ```bash
   git clone <repository_url>
   cd final_project
   ```

2. **Install dependencies:**
   ```bash
   pip install flask requests pylint
   ```

3. **Run Unit Tests:**
   ```bash
   python test_emotion_detection.py
   ```

4. **Start the Flask Application:**
   ```bash
   python server.py
   ```
   Open your browser and navigate to `http://localhost:5000`.

5. **Run Static Code Analysis:**
   ```bash
   pylint server.py
   ```

---

## Author

- **Course:** Developing AI Applications with Python and Flask
- **Developer:** Samarth
