# Grade-O-Meter: AI-Powered Supply Chain Quality Standardization

##  Project Overview
Grade-O-Meter is an **Edge-AI Logistics Dashboard** that solves "Information Asymmetry" in rural supply chains. It digitizes subjective quality checks into objective data using Computer Vision and Geolocation.

**Live Demo:** [Click Here to Open App](https://GPaul02.github.io/Grade-O-Meter/)

Technical Summary:
Grade-O-Meter is a fully client-side web application developed using TensorFlow.js for real-time image inference. All processing takes place on the user’s device, resulting in:
	•	No dependency on backend servers
	•	Low inference latency suitable for remote rural environments
	•	Full data privacy since images do not leave the device

Getting Started:
Requirements:
• A modern web browser (Chrome, Firefox, Edge, Safari)
• Internet connection required for initial loading only
• Permission for webcam access (for image-based inspection)
• Permission for location access (for geo-tagging)

Installation:
	1.	Clone the repository:
      git clone https://github.com/GPaul02/Grade-O-Meter.git
	2.	Navigate to the directory:
      cd Grade-O-Meter
	3.	Open the file “index.html” in your browser to run the application locally.

Environment Details:
This solution uses edge computing and does not require any server-side environment variables.
• No external API keys
• No cloud dependencies
• Local session storage used for temporary data
• Model is stored as a local file (model.json)

License:
This project is released under the MIT License. Refer to the LICENSE file for detailed terms and usage rights.
