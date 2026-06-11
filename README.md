# 🤟 Vocalink (Sign Language to Text & Speech Conversion System)

<div align="center">

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-orange)
![CustomTkinter](https://img.shields.io/badge/GUI-CustomTkinter-purple)
![License](https://img.shields.io/badge/License-MIT-yellow)

### Real-Time Sign Language Recognition Using Computer Vision and Deep Learning

Convert hand gestures into text and speech in real time using a webcam, deep learning, and an interactive graphical user interface.

</div>

---

# 📖 Table of Contents

- [Overview](#-overview)
- [Problem Statement](#-problem-statement)
- [Solution](#-solution)
- [Features](#-features)
- [System Architecture](#-system-architecture)
- [Project Workflow](#-project-workflow)
- [Technology Stack](#-technology-stack)
- [Software Requirements](#-software-requirements)
- [Hardware Requirements](#-hardware-requirements)
- [Project Structure](#-project-structure)
- [Dataset Collection Module](#-dataset-collection-module)
- [Gesture Recognition Module](#-gesture-recognition-module)
- [GUI Application Module](#-gui-application-module)
- [Installation](#-installation)
- [Usage](#-usage)
- [Model Information](#-model-information)
- [Supported Gestures](#-supported-gestures)
- [Applications](#-applications)
- [Future Enhancements](#-future-enhancements)
- [Screenshots](#-screenshots)
- [Contributing](#-contributing)
- [License](#-license)
- [Author](#-author)

---

# 🎯 Overview

Sign language is one of the most important communication methods for people with hearing and speech impairments. However, communication barriers still exist because many people do not understand sign language.

This project introduces a **real-time Sign Language to Text and Speech Conversion System** that utilizes:

- Computer Vision
- Hand Tracking
- Deep Learning
- Text-to-Speech Technology
- Modern Graphical User Interface

The system detects hand gestures through a webcam, classifies them using a trained deep learning model, displays the corresponding text, and converts the recognized text into speech.

The goal is to provide a simple, accessible, and efficient communication solution.

---

# ❗ Problem Statement

Individuals who communicate through sign language often face challenges when interacting with people who do not understand sign language.

Existing communication methods may require:

- Human interpreters
- Specialized devices
- Manual translation

These solutions can be expensive, inaccessible, or inconvenient.

There is a need for a cost-effective, real-time system capable of translating hand gestures into understandable text and speech.

---

# 💡 Solution

The proposed system uses a webcam to capture hand gestures and applies computer vision and deep learning techniques to recognize them.

The recognized gesture is:

1. Detected
2. Classified
3. Converted to text
4. Converted to speech

This enables effective communication between sign language users and non-sign language users.

---

# ✨ Features

### Real-Time Hand Detection
Detects hand gestures using a webcam.

### Deep Learning-Based Recognition
Uses a trained Keras model to classify gestures accurately.

### Sign Language to Text Conversion
Displays recognized gestures instantly as text.

### Text-to-Speech Output
Converts recognized text into audible speech.

### Modern GUI
Built using CustomTkinter for an attractive user experience.

### Confidence-Based Prediction
Filters weak predictions to improve reliability.

### Easy Dataset Expansion
Allows adding new gestures and retraining the model.

### Lightweight & Fast
Runs efficiently on standard computers.

---

# 🏗️ System Architecture

```text
Webcam
   │
   ▼
Hand Detection
   │
   ▼
Image Preprocessing
   │
   ▼
Deep Learning Model
   │
   ▼
Gesture Classification
   │
   ├────────► Text Output
   │
   ▼
Text-to-Speech Engine
   │
   ▼
Audio Output
```

---

# 🔄 Project Workflow

## Phase 1: Dataset Collection

- Capture hand images using webcam
- Detect hand region
- Crop hand image
- Normalize image size
- Save gesture images

---

## Phase 2: Model Training

- Prepare dataset
- Train deep learning model
- Export model as:

```text
keras_model.h5
```

- Generate:

```text
labels.txt
```

---

## Phase 3: Gesture Recognition

- Detect hand
- Preprocess image
- Predict gesture
- Display result

---

## Phase 4: Text & Speech Conversion

- Show prediction on GUI
- Convert text to speech
- Provide user interaction controls

---

# 🛠 Technology Stack

## Programming Language

- Python 3.9+

## Computer Vision

- OpenCV

## Hand Tracking

- CVZone

## Machine Learning

- TensorFlow
- Keras

## GUI Development

- CustomTkinter

## Image Processing

- Pillow (PIL)
- NumPy

## Speech Processing

- pyttsx3

---

# 💻 Software Requirements

| Software | Version |
|-----------|-----------|
| Python | 3.9+ |
| OpenCV | Latest |
| TensorFlow | 2.x |
| CVZone | Latest |
| NumPy | Latest |
| Pillow | Latest |
| CustomTkinter | Latest |
| pyttsx3 | Latest |

---

# 🖥 Hardware Requirements

### Minimum

- Intel i3 Processor
- 4 GB RAM
- Webcam
- 500 MB Storage

### Recommended

- Intel i5/i7 Processor
- 8 GB RAM
- HD Webcam
- SSD Storage

---

# 📁 Project Structure

```text
Sign-Language-To-Text-And-Speech/
│
├── Dataset/
│   ├── Bathroom/
│   ├── Drink/
│   ├── Eat/
│   ├── Goodbye/
│   ├── HII/
│   ├── Hungry/
│   ├── I_love_you/
│   ├── NO/
│   ├── Okay/
│   ├── Play/
│   ├── Please/
│   ├── Sorry/
│   ├── Thanks/
│   └── YES/
│
├── Model/
│   ├── keras_model.h5
│   └── labels.txt
│
├── DataCollection.py
├── GestureRecognition.py
├── GUI_Application.py
│
├── requirements.txt
├── LICENSE
└── README.md
```

---

# 📸 Dataset Collection Module

This module is responsible for collecting gesture images.

### Functions

- Webcam access
- Hand detection
- Image cropping
- Background normalization
- Dataset generation

### Output

```text
Gesture Images Dataset
```

---

# 🧠 Gesture Recognition Module

This module performs real-time gesture classification.

### Functions

- Detect hand
- Process image
- Load trained model
- Predict gesture
- Display output

### Output

```text
Predicted Gesture Label
```

---

# 🖥 GUI Application Module

Provides an interactive interface.

### Buttons

| Button | Function |
|----------|-----------|
| Start | Start Camera |
| Stop | Stop Camera |
| Speak | Convert Text to Speech |
| Clear | Clear Output |

### Features

- Live camera feed
- Text display
- Speech generation
- User-friendly interaction

---

# ⚙️ Installation

## Clone Repository

```bash
git clone https://github.com/amansatidata/Sign-Language-To-Text-And-Speech.git
cd Sign-Language-To-Text-And-Speech
```

## Create Virtual Environment

```bash
python -m venv venv
```

## Activate Environment

### Windows

```bash
venv\Scripts\activate
```

### Linux / macOS

```bash
source venv/bin/activate
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Usage

### Run Dataset Collection

```bash
python DataCollection.py
```

### Run Gesture Recognition

```bash
python GestureRecognition.py
```

### Run GUI Application

```bash
python GUI_Application.py
```

---

# 🤖 Model Information

| Property | Value |
|-----------|--------|
| Model Type | CNN-based Image Classifier |
| Framework | TensorFlow/Keras |
| Input Size | 300×300 |
| Output | Gesture Label |
| Detection Method | CVZone Hand Tracking |

---

# ✋ Supported Gestures

- Bathroom & Restroom
- Book
- Call & Number
- Dislike
- Done
- Drink
- Eat
- Goodluck
- Goodbye
- HII
- Heart
- Help
- Hungry
- Hurt
- I hate you
- I Love You
- I
- Looser
- More
- NO
- Okay
- One Thing
- Peace
- Play
- Please
- Punch
- Question
- Sit Down
- Sorry
- Stand
- Stop
- Thanks
- Water
- YES

---

# 🌍 Applications

- Sign Language Interpretation
- Assistive Communication
- Human-Computer Interaction
- Accessibility Systems
- Educational Platforms
- Smart Healthcare Solutions
- Interactive Learning Systems

---

# 🚀 Future Enhancements

- Dynamic gesture recognition
- Sentence formation
- Multi-language speech support
- Mobile application deployment
- Cloud-based inference
- Higher accuracy models
- Multi-hand recognition
- Real-time translation

---



# 🤝 Contributing

Contributions are welcome.

1. Fork the repository
2. Create a branch

```bash
git checkout -b feature-name
```

3. Commit changes

```bash
git commit -m "Add new feature"
```

4. Push changes

```bash
git push origin feature-name
```

5. Open a Pull Request

---

# 📜 License

This project is licensed under the MIT License.

See the LICENSE file for complete information.

---

# 👨‍💻 Author

**Aman Sati**

B.Tech Student | Computer Science and Engineering

### Skills

- Python Development
- Machine Learning
- Deep Learning
- Computer Vision
- AI-Based Applications

- GitHub: https://github.com/amansatidata
LinkedIn: https://linkedin.com/in/aman-sati-1801a729a

---

# ⭐ Support

If you found this project useful:

⭐ Star the repository

🍴 Fork the repository

📝 Share feedback

🐞 Report issues

---

<div align="center">

### 🤟 Empowering Communication Through Artificial Intelligence

Made with ❤️ using Python, Computer Vision, and Deep Learning

</div>
