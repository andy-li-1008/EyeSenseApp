# EyeSenseApp
An AI-Powered Solution for Driver Safety
# EyeSense: AI-Powered Driver Safety Assistant

[![Platform: Android](https://img.shields.io/badge/Platform-Android-green.svg)](https://www.android.com/)
[![Built with MIT App Inventor](https://img.shields.io/badge/Built%20with-MIT%20App%20Inventor-orange.svg)](https://appinventor.mit.edu/)

**EyeSense** is an innovative Android application that uses real-time AI to detect driver drowsiness and aggressive driving patterns, helping prevent accidents before they happen. The app acts as your intelligent co-pilot, monitoring your state through your phone's camera and microphone.

---

## 🌟 Key Features

- **Real-Time Drowsiness Detection**: Uses computer vision to analyze eye closure (PERCLOS), yawning frequency, and head pose.
- **Multi-Index Fusion Algorithm**: Combines multiple visual cues for robust detection, even in challenging conditions (e.g., sunglasses).
- **AI Buddy Intervention**: Provides corrective, non-jarring alerts via sound, vibration, or voice prompts.
- **Lightweight & Efficient**: Built with MobileNet architecture for optimal performance on mobile devices.
- **Privacy-First Design**: All processing happens locally on your device—no video or audio data is uploaded to the cloud.

---

## 📱 Download & Installation

###  Direct APK Download (Recommended for Testing)
1. Download the latest `EyeSense.apk` file to your Android device.
2. On your phone, enable **"Install from Unknown Sources"** in Settings → Security.
3. Open the downloaded `.apk` file and follow the installation prompts.

---

## 🚀 How to Use

1. **Mount your phone** securely on the dashboard or a holder, ensuring the front camera has a clear view of your face.
2. **Launch EyeSense** and grant the necessary permissions (camera, microphone).
3. **Start a drive session** by tapping the "Start Monitoring" button.
4. Drive normally. The app will run in the background and provide alerts if drowsiness or aggression is detected.
5. When an alert sounds, please find a safe place to pull over and rest.

---

## 🛠️ Technical Architecture
User's Phone (Android)
├── MIT App Inventor Frontend
│ ├── Camera Feed Capture
│ 
│ ├── Alert System (Visual/Audio/Vibration)
│ └── User Interface
└── Local AI Engine (Python/TFLite)
├── Face Detection (MTCNN/CNN)
├── Eye State Classification (Open/Closed)
├── Mouth State Classification (Normal/Yawn)
├── Head Pose Estimation
├── Fatigue Score Fusion Algorithm


text

### AI Models & Training
- **Visual Model**: Custom CNN trained on combined datasets (Closed Eyes, Yawn, Head Pose).
  
  
- **Training Data**: Custom collected datasets.

## 📊 Performance & Validation

Our AI models were rigorously validated using train/validation splits:

- **Drowsiness Detection (Visual)**: **96% accuracy** on validation set
- **Emotion Recognition (Audio)**: ~68% accuracy (under improvement)
- **Real-Time Performance**: Processes ~15-20 FPS on mid-range Android devices

---

## 👥 Who Benefits?

- **Everyday Drivers & Passengers**: For personal vehicle safety.
- **Commercial Fleets**: Trucking, delivery, and transport companies.
- **Young Drivers**: Ages 16–25, who are statistically at higher risk.
- **Ride-Share & Taxi Drivers**: Professional drivers with long hours.
- **Families**: Parents concerned about teen driving safety.

---

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **Report Bugs**: Open an issue with detailed steps to reproduce.
2. **Suggest Features**: Share your ideas for new alerts, metrics, or UI improvements.
3. **Improve Models**: Contribute to better datasets or optimized TFLite models.
4. **Localization**: Help translate the app into other languages.


---

## ❓ Frequently Asked Questions

**Q: Does EyeSense work at night?**  
A: Performance may be reduced in low-light conditions. We recommend using the phone's "screen fill light" or ensuring adequate cabin lighting.

**Q: Is my data being uploaded or stored?**  
A: No. All processing is done locally on your device. No video or audio leaves your phone.

**Q: Can it work with sunglasses?**  
A: Yes! Our multi-index fusion can rely more on head pose and yawning detection when eyes are obscured.

**Q: What Android versions are supported?**  
A: Android 8.0 (Oreo) and above.

**Q: Why does the app need microphone permission?**  
A: This is used only for the aggressive driving detection module. You can disable it in settings if desired.

---

## ⚖️ Ethical Considerations & Privacy

We are committed to **Responsible AI**:
- **Transparency**: This project is fully open-source.
- **Bias Mitigation**: We strive to use diverse training datasets.
- **User Control**: Alerts are advisory; the driver maintains full agency.
- **Privacy by Design**: No cloud storage or data sharing.

---

## 🧑‍💻 Developers & Team

- **Andy Li** – AI Model Development, Mobile App Development, System Integration, Video Creation
- **Alex Xu** – UI/UX, Testing

This project was created for the demonstrating how AI can be applied for social good.

---

## 📚 Learn More

- **Video Demo**: [Watch on YouTube](https://youtu.be/_HQNEgt6g2k)
- **Project Poster**: [View PowerPoint](https://github.com/andy-li-1008/EyeSenseApp/blob/main/Poster-eyesense.pptx)



---

## 🙏 Acknowledgments

- MIT App Inventor team for the incredible development platform.
- Open-source communities for TensorFlow, OpenCV, and Librosa.
- Public dataset providers for making training data accessible.
- Our mentors, teachers, and families for their unwavering support.

---

**Drive safely. Let EyeSense be your guardian on the road.** 🛡️🚗
