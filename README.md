Indian Sign Language Recognition System
A real-time Indian Sign Language (ISL) recognition system built using Python, CNN (Convolutional Neural Networks), MediaPipe, and Tkinter GUI. This project is designed to bridge the communication gap between speech-impaired individuals and others by translating hand gestures into readable and spoken language.

🧠 Features
✋ Real-time hand gesture recognition using webcam.
🧠 Trained CNN model on A-Z and 0-9 ISL signs with two-hand support.
📷 MediaPipe integration for 2-hand landmark detection (42 landmarks).
💬 Automatic word segmentation and sentence formation from alphabet gestures.
🔊 Text-to-speech conversion of recognized sentences.
🎙️ Speech-to-sign mode: converts spoken words into animated ISL signs.
🎨 Fullscreen Tkinter GUI with dark mode and interactive buttons.
💡 Word auto-complete and suggestions based on gesture prefixes.


🗂️ Project Structure
Indian-Sign-Language-main/
│
├── model/                      # Trained CNN model (.h5) and LabelEncoder (.pkl)
├── images/                    # ISL images for A-Z and 0-9
├── utils/                     # Helper scripts for preprocessing, landmark extraction
├── main.py                    # Main GUI launcher
├── real_time_recognition.py   # Real-time prediction logic using OpenCV + MediaPipe
├── speech_to_sign.py          # Speech-to-sign animation logic
├── preprocess.py              # Data preparation and pickle saving
├── README.md                  # Project documentation
└── requirements.txt           # Python dependencies


🚀 Getting Started
1. Clone the Repository
git clone https://github.com/your-username/Indian-Sign-Language.git
cd Indian-Sign-Language-main

2. Install Requirements
pip install -r requirements.txt

3. Run the App
python main.py

💻 Technologies Used
Python
OpenCV
MediaPipe
TensorFlow / Keras
Tkinter
gTTS for text-to-speech
SpeechRecognition for speech input


📊 Model Info
Input: Normalized (42, 2, 1) hand landmark features.

Output: 35 classes (A-Z + 0-9).

Data: Augmented dataset with 6 variations per image for robustness.


🤝 Acknowledgements
Inspired by the vision to help those who are speech or hearing impaired by enabling two-way communication through sign language.


📌 Future Scope
>Mobile app using Kivy or Flutter + Flask.
>Support for word/phrase-level ISL.
>Sentence translation accuracy enhancement.
>Multilingual speech-to-sign support.

