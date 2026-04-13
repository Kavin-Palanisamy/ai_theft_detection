📌 Overview

This project is an AI-powered theft detection system that uses real-time object detection to identify human presence and instantly send alerts via Telegram.

It leverages computer vision with YOLOv8 and integrates with the Telegram Bot API to notify users with messages and images.

🎯 Features
  ✅ Real-time human detection using webcam
  ✅ AI-based detection with high accuracy
  ✅ Instant Telegram alerts (message + photo)
  ✅ Cooldown system to prevent spam alerts
  ✅ Simple and lightweight implementation

🧠 How It Works

  Webcam captures live video feed
  YOLOv8 model processes each frame
  Detects objects and identifies humans
  If a person is detected:
  Snapshot is saved
  Telegram alert is sent
  Image is shared via bot
  Cooldown prevents repeated alerts

🛠️ Technologies Used
  🐍 Python
  🎥 OpenCV (cv2)
  🤖 Ultralytics YOLOv8
  🌐 Requests (API communication)
  📩 Telegram Bot API
  📦 Requirements

Install dependencies using:

pip install ultralytics opencv-python requests

⚙️ Setup Instructions

2️⃣ Setup Telegram Bot
Create a bot using BotFather
Get your BOT_TOKEN
Get your CHAT_ID

Replace in code:

BOT_TOKEN = "YOUR_BOT_TOKEN"
CHAT_ID = "YOUR_CHAT_ID"

⚠️ Important: Never share your bot token publicly.

3️⃣ Run the Project
python main.py

Press Q to exit.

📸 Output
Displays live webcam feed with bounding boxes
Sends:
📩 Alert message
📷 Snapshot image
🔒 Security Note

⚠️ Your current code contains a hardcoded Telegram bot token.
For safety:

Regenerate your token via BotFather
Store it in .env file instead of code
🚀 Future Enhancements
🔍 Face recognition using OpenCV
☁️ Cloud storage for images
📱 Mobile app integration
🧠 Intruder classification (known vs unknown)
📡 IoT hardware integration (ESP32 + sensors)
📄 Project Structure
📁 theft-detection-yolo
 ├── main.py
 ├── snapshot.jpg
 ├── README.md
 └── requirements.txt
🎯 Use Cases
🏠 Home security
🏢 Office surveillance
🏭 Industrial monitoring
🚗 Parking area monitoring
