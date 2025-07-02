# ESP32-CAM Firebase Image Uploader

This project uses an **ESP32-CAM** to capture images, encode them in **Base64**, and upload them to **Firebase Realtime Database** every 10 seconds.

---

##  Features

- Captures an image using the ESP32-CAM.
- Encodes the image to **Base64** using `mbedtls`.
- Uploads the image string to Firebase under `/esp32-cam/`.
- Prints logs to the **Serial Monitor** for debugging.

---

##  Requirements

- ESP32-CAM board (AI-Thinker module)
- Arduino IDE with ESP32 board support
- Firebase Realtime Database setup
- PSRAM-enabled ESP32 board recommended

---

##  Libraries Used

- `FirebaseESP32` by Mobizt  
- `mbedtls` for Base64 encoding (included with ESP32)
- `esp_camera` (ESP32 core)
- `WiFi.h`

---

##  Setup

1. Clone or download the repo.
2. Open the `.ino` file in Arduino IDE.
3. Install dependencies (via **Library Manager**).
4. Replace the following in the code:
   - `ssid` and `password` → Your WiFi credentials  
   - `FIREBASE_HOST`, `FIREBASE_API_KEY`, `USER_EMAIL`, `USER_PASSWORD` → Your Firebase details  
5. Flash the code to your ESP32-CAM.
6. Open Serial Monitor at **115200 baud**.


