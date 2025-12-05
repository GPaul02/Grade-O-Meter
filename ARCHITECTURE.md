# Technical Architecture Document

## 1. System Overview
Grade-O-Meter is a client-side web application designed for offline inference. It utilizes a **Single Page Application (SPA)** architecture where the AI model is loaded directly into the browser's memory, eliminating latency and server costs.

## 2. Architectural Diagram

[ User Device (Smartphone/Laptop) ]
         |
         | (1. Request App)
         v
[ GitHub Pages (Static Host) ]
         |
         | (2. Delivers HTML/JS/Assets)
         v
[ Browser Runtime Environment ]
    |
    +--- [ UI Layer (HTML5/Bootstrap) ] <-----> [ DOM Updates (Dashboard) ]
    |
    +--- [ Logic Layer (JavaScript) ]
    |       |
    |       +--- [ Geolocation API ] (Fetches GPS)
    |       +--- [ TensorFlow.js Engine ]
    |                  ^
    |                  | (3. Loads Model)
    |                  v
    |            [ MobileNet Model Files (JSON/Bin) ]
    |
    +--- [ Input Layer ]
            |
            +--- [ Webcam Feed ] OR [ File Upload ]

## 3. Data Flow
1.  **Input:** User captures image via Webcam or Upload.
2.  **Preprocessing:** Image is resized to 224x224 and normalized.
3.  **Inference:** TensorFlow.js runs the MobileNet model against the input.
4.  **Post-Processing:** The class with the highest probability (>80%) determines the Grade.
5.  **Logging:** The result, timestamp, and GPS coordinates are logged to the batch array.

## 4. Tech Stack
* **Frontend:** HTML5, CSS3, Bootstrap 5.
* **AI Framework:** TensorFlow.js (Client-side).
* **Model Architecture:** Transfer Learning on MobileNet.
* **Deployment:** GitHub Pages.
