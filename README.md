# Deepfake Detection Tool 🕵‍♂

## Overview
The Deepfake Detection Tool is a desktop application built using Python and Tkinter that allows users to upload an image or video and check for deepfake content. The application integrates with an external deepfake detection API to analyze the uploaded media.

## Features
- 🖱 User-friendly interface for uploading files.
- 📷 Supports image and video formats (.png, .jpg, .jpeg, .mp4, .mov).
- 🔍 Processes images/videos and sends them to a deepfake detection API.
- 📊 Displays results with deepfake probability.
- 🔄 Reset functionality to clear previous selections.

## Technologies Used
- 🐍 Python (Main programming language)
- 🖥 Tkinter (GUI framework)
- 🖼 OpenCV (cv2) (Image processing)
- 📊 NumPy (Array manipulation)
- 🌐 Requests (API calls)

## Architecture
### User Interaction Layer
- Tkinter GUI for file selection, submission, and reset.
- Labels to display selected file paths and results.

### Processing Layer
- Reads and preprocesses images and video frames.
- Resizes images to 224x224 pixels for consistency.

### API Communication Layer
- Converts images to byte format.
- Sends POST requests to the deepfake detection API.
- Parses and displays results received from the API.

## Installation
### Prerequisites
Ensure you have Python installed on your system. You also need to install the required dependencies.

```bash
pip install opencv-python numpy requests
