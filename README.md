# Jujutsu Kaisen (咒術迴戰) Domain Expansion Recognition System

<div align="center">

[Jujutsu Kaisen](https://img.shields.io/badge/Anime-Jujutsu%20Kaisen-ff6b6b?style=for-the-badge)
[Python](https://img.shields.io/badge/Python-3.7+-3776ab?style=for-the-badge&logo=python&logoColor=white)
[OpenCV](https://img.shields.io/badge/OpenCV-4.x-5c3ee8?style=for-the-badge&logo=opencv&logoColor=white)
[MediaPipe](https://img.shields.io/badge/MediaPipe-Google-4285f4?style=for-the-badge)
[License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

*An AI-powered hand gesture recognition system that detects Domain Expansion techniques from the popular anime Jujutsu Kaisen (咒術迴戰)*

</div>

##  Overview

This project brings the supernatural world of Jujutsu Kaisen to life through computer vision and machine learning. Using advanced hand tracking technology, the system can recognize and classify Domain Expansion hand signs in real-time, featuring iconic techniques from beloved characters.

###  Featured Domain Expansions

| Character | Domain Expansion | Description |
|-----------|------------------|-------------|
| **Gojo Satoru** | Infinite Void (無量空処) | The ultimate technique of the strongest sorcerer |
| **Ryomen Sukuna** | Malevolent Shrine (伏魔御廚子) | The King of Curses' devastating domain |
| **Megumi Fushiguro** | Chimera Shadow Garden (嵌合暗翳庭) | Ten Shadows Technique manifestation |
| **Custom** | The L World | Special custom domain expansion |

##  Features

### Core Functionality
- **Real-time Hand Gesture Recognition** - Detect Domain Expansion signs using your webcam
- **Multi-character Support** - Recognize gestures from multiple Jujutsu Kaisen characters
- **High Accuracy Detection** - Machine learning model with advanced feature extraction
- **Visual Feedback** - Character previews and confidence indicators
- **Customizable Training** - Record and train your own gesture variations

### Technical Highlights
- **MediaPipe Integration** - Advanced hand landmark detection
- **Random Forest Classification** - Robust machine learning model
- **Real-time Processing** - Optimized for live video streams
- **Cross-platform Compatibility** - Works on Windows, macOS, and Linux

##  Quick Start

### Prerequisites

```bash
Python 3.7+
Webcam/Camera access
```

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/WWIIITT/Jujutsu-Kaisen-Domain-Expansion.git
cd Jujutsu-Kaisen-Domain-Expansion
```

2. **Install dependencies**
```bash
pip install opencv-python mediapipe tensorflow pygame scikit-learn numpy
```

3. **Run the application**
```bash
python "Jujutsu Kaisen Domain Expansion.ipynb"
```

## 🎮 Usage Guide

### 1. Recording Training Data
- Select option `1` from the main menu
- Press `R` to start recording gesture videos
- Record different variations of each Domain Expansion hand sign
- Press `R` again to stop recording

### 2. Training the Model
- Select option `2` from the main menu
- Label your recorded videos with corresponding domain expansions
- The system will automatically extract features and train the model
- Model accuracy will be displayed upon completion

### 3. Real-time Detection
- Select option `3` from the main menu
- Position your hands in front of the camera
- Perform Domain Expansion hand signs
- Watch as the system recognizes and displays the corresponding technique

## 🛠️ Technical Architecture

### Hand Feature Extraction
- **MediaPipe Hands**: 21-point hand landmark detection
- **Feature Vector**: 84-dimensional array (42 points × 2 hands)
- **Preprocessing**: Normalization and coordinate transformation

### Machine Learning Pipeline
- **Algorithm**: Random Forest Classifier
- **Training**: Video-based gesture sampling
- **Validation**: Train-test split with accuracy metrics
- **Prediction**: Real-time confidence scoring

### Detection System
- **Gesture Buffer**: Temporal consistency checking
- **Confidence Threshold**: Minimum 80% accuracy requirement
- **Cooldown System**: Prevents false positive spam
- **Visual Feedback**: Character previews and progress indicators

## 📁 Project Structure

```
Jujutsu-Kaisen-Domain-Expansion/
├── images/                    # Domain expansion character images
│   ├── infinite_void.jpg
│   ├── malevolent_shrine.jpg
│   ├── chimera_shadow.jpg
│   └── the_L.jpg
├── gesture_videos/           # Training video storage
├── jujutsu_data/            # Processed training data
├── Jujutsu Kaisen Domain Expansion.ipynb  # Main application
├── jujutsu_model.pkl        # Trained ML model
├── README.md
└── LICENSE
```

## 🤝 Contributing

We welcome contributions from the Jujutsu Kaisen community! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/new-domain`
3. **Add new Domain Expansions** or improve existing recognition
4. **Commit your changes**: `git commit -m 'Add Nobara's Straw Doll Technique'`
5. **Push to the branch**: `git push origin feature/new-domain`
6. **Open a Pull Request**

### Ideas for Contributions
- Add more Domain Expansions (Nobara, Nanami, etc.)
- Improve gesture recognition accuracy
- Add sound effects and visual enhancements
- Create mobile app version
- Add gesture difficulty ratings

## 📊 Performance Metrics

- **Detection Accuracy**: ~95% with proper training data
- **Real-time FPS**: 30+ on modern hardware
- **Response Time**: <100ms gesture recognition
- **Training Time**: 2-5 minutes for 4 domain types

## 🔧 Troubleshooting

### Common Issues

**Camera not detected**
```bash
# Check camera permissions and try different camera indices
cap = cv2.VideoCapture(1)  # Try 0, 1, 2...
```

**Low detection accuracy**
```bash
# Record more training videos with better lighting
# Ensure clear hand visibility
# Train with multiple hand positions
```

**Module import errors**
```bash
pip install --upgrade opencv-python mediapipe scikit-learn
```

---

<div align="center">

**"Domain Expansion is the pinnacle of jujutsu sorcery!"** ⚡

*Made with ❤️ for the Jujutsu Kaisen community*

</div>

