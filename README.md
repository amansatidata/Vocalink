# 🤟 Vocalink (Sign Language to Text & Speech Conversion System)

A real-time AI-powered communication system that translates sign language gestures into text and speech using Computer Vision, Deep Learning, and Natural Human-Computer Interaction.

## Key Highlights

- Real-time hand gesture recognition using webcam input
- Deep learning-based classification model
- Automatic conversion of gestures to text
- Text-to-speech functionality for enhanced accessibility
- Modern GUI built with CustomTkinter
- Designed to support communication for individuals with hearing and speech impairments

  

- ## Demo

### Live Gesture Recognition
Detects hand gestures in real time and displays the predicted sign.

### Text Conversion
Recognized gestures are instantly converted into readable text.

### Speech Output
Generated text can be spoken aloud using the integrated Text-to-Speech engine.




## System Architecture

Webcam Input
        │
        ▼
Hand Detection (CVZone)
        │
        ▼
Image Preprocessing
        │
        ▼
Deep Learning Model (TensorFlow/Keras)
        │
        ▼
Gesture Classification
        │
        ├──► Text Output
        │
        ▼
Text-to-Speech Engine
        │
        ▼
Audio Output






## Technical Features

### Computer Vision
- Real-time hand detection and tracking
- ROI extraction with boundary handling
- Aspect ratio preserving image normalization

### Deep Learning
- CNN-based gesture classification
- Confidence-based prediction filtering
- Support for custom gesture datasets

### User Interface
- Interactive GUI
- Live camera feed
- Real-time prediction display
- Speech generation controls

### Accessibility
- Gesture-to-text conversion
- Text-to-speech output
- Improved communication support





## Technology Stack

| Category | Technology |
|-----------|-----------|
| Programming Language | Python |
| Computer Vision | OpenCV, CVZone |
| Deep Learning | TensorFlow, Keras |
| GUI Framework | CustomTkinter |
| Image Processing | NumPy, Pillow |
| Speech Processing | pyttsx3 |
| Hardware | Webcam |





## Results

The system successfully:

- Detects hand gestures in real time
- Classifies gestures using a trained deep learning model
- Converts recognized gestures into text
- Generates speech output from recognized text
- Provides a user-friendly interface for interaction

Supported Gesture Classes: 14

- Bathroom & Restroom
- Book
- Call & Number
- Dislike
- Done
- Drink
- Eat
- GoodLuck
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





## Future Enhancements

- Dynamic sign language recognition
- Sentence generation from continuous gestures
- Multi-language speech synthesis
- Mobile application deployment
- Cloud-based inference and scalability
- Support for larger sign language vocabularies
- Real-time translation systems




## Author

**Aman Sati**

B.Tech Student | Computer Science and Engineering

### Areas of Interest
- Artificial Intelligence
- Machine Learning
- Deep Learning
- Computer Vision
- Human-Computer Interaction

GitHub: https://github.com/amansatidata
LinkedIn: https://linkedin.com/in/aman-sati-1801a729a




# 📜 License

This project is licensed under the MIT License.
