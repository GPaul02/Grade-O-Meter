# Grade-O-Meter: AI-Powered Supply Chain Quality Standardization

##  Project Overview
Grade-O-Meter is an **Edge-AI Logistics Dashboard** that solves "Information Asymmetry" in rural supply chains. It digitizes subjective quality checks into objective data using Computer Vision and Geolocation.

**Live Demo:** [Click Here to Open App](https://GPaul02.github.io/Grade-O-Meter/)

## Setup & Installation
This project is designed as a **Client-Side Web Application** running via TensorFlow.js. It requires no backend server installation.

### Prerequisites
* A modern web browser (Chrome, Edge, Firefox, Safari).
* Active internet connection (for initial load only).
* Webcam permissions allowed.
* Location permissions allowed (for Geo-tagging).

### Installation Steps
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/GPaul02/Grade-O-Meter.git](https://github.com/GPaul02/Grade-O-Meter.git)
    ```
2.  **Navigate to the folder:**
    ```bash
    cd Grade-O-Meter
    ```
3.  **Run Locally:**
    Simply double-click `index.html` to open it in your browser.

##  Environment Variables
Since this application uses **Edge Computing** (Client-Side Inference), no server-side environment variables are required.
* **API Keys:** None (No external cloud calls).
* **Database:** Local Session Storage (RAM).
* **Model Path:** Hardcoded relative path (`./model.json`).

##  License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
