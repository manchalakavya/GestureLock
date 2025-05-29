
# GestureLock

**GestureLock** is a real-time, gesture-based human authentication system. This project replaces traditional authentication methods (like passwords or ID cards) with dynamic hand gestures, offering a secure, contactless, and personalized way to verify identity using computer vision and deep learning.

Built with Python, OpenCV, MediaPipe, and TensorFlow, GestureLock tracks user-specific hand movements via webcam and verifies identity through a trained gesture recognition model.

---

## 🔍 Why GestureLock?

Traditional authentication methods are either easy to forget (passwords) or inconvenient (ID cards, biometrics). **GestureLock** offers:

- **Contactless verification** — ideal for hygienic environments  
- **Highly personalized security** — gestures are harder to fake than static patterns  
- **Real-time processing** — authentication happens in milliseconds  
- **Scalability** — works with webcams, IP cameras, or edge devices  

---

## 💡 How It Works

1. **Data Collection**  
   Users perform unique hand gestures in front of a webcam. Landmark data is recorded using MediaPipe.

2. **Model Training**  
   The time-series gesture data is used to train an LSTM-based deep learning model.

3. **Authentication**  
   In real time, the system matches a user’s gesture to trained profiles and verifies access accordingly.

---

## 🛠️ Technologies Used

| Tool               | Purpose                                     |
|--------------------|---------------------------------------------|
| Python 3.x         | Core programming                            |
| OpenCV             | Webcam input and frame processing           |
| MediaPipe          | Hand landmark detection                     |
| TensorFlow/Keras   | Gesture recognition model                   |
| NumPy              | Data formatting and vectorization           |
| Tkinter (optional) | GUI interface for user interaction          |

---

## 🚀 Getting Started

### 1. Install Dependencies

```bash
git clone https://github.com/yourusername/GestureLock.git
cd GestureLock
pip install -r requirements.txt
```

### 2. Collect Gesture Data

```bash
python collect-data.py
```

### 3. Train the Model

```bash
python train-model.py
```

### 4. Run Real-Time Authentication

```bash
python authentication.py
```

### 5. (Optional) Launch the GUI

```bash
python gui.py
```

---

## 📂 Project Structure

```
GestureLock/
├── Data/                     # Gesture sequence data per user
├── Model/                    # Trained model files
├── collect-data.py           # For capturing gesture sequences
├── train-model.py            # Model training using LSTM
├── authentication.py         # Real-time gesture-based verification
├── gui.py                    # Optional GUI interface
├── utils.py                  # Helper functions
├── requirements.txt          # Required libraries
└── README.md                 # Project documentation
```

---

## ✨ Key Features

- 📷 **Live Gesture Capture** using webcam and MediaPipe  
- 🧠 **Temporal Gesture Recognition** with LSTM model  
- 🔐 **Custom User Registration** and model training  
- ⚡ **Fast and Lightweight** — suitable for local or edge deployment  
- 🧩 **Modular Codebase** — easily extendable for attendance or access control  

---

## 🔮 Future Improvements

- Multi-gesture authentication per user  
- Integration with smart locks and IoT systems  
- Cloud-based login support via APIs  
- Gesture combination sequences as passcodes  
- Enhanced GUI for user and admin access  

---

## 🙋‍♂️ Author

Created and maintained by **Kavya Manchala**  
GitHub Profile → [(manchalakavya) https://github.com/manchalakavya)

---

## 📄 License

This project is licensed under the **MIT License**.  
Feel free to use, improve, and share it with proper credit.

---

> “Your hand is your password. Move with purpose, unlock with confidence.” — **GestureLock**
