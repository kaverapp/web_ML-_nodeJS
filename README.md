`Real-Time Object Detection with COCO-SSD`

This project demonstrates real-time object detection using the COCO-SSD model in a web application. It utilizes JavaScript, HTML, and CSS to access the user's webcam, detect objects in the camera's view, and highlight them with bounding boxes and confidence scores.

🚀 Features

Uses the COCO-SSD machine learning model for object detection

Real-time webcam stream processing

Displays detected objects along with their confidence scores

Highlights objects in the live video feed with bounding boxes

🛠️ Technologies Used

JavaScript: For implementing webcam access, COCO-SSD model loading, and object detection logic

HTML: For structuring the webpage with necessary elements like buttons and video stream

CSS: For styling the webpage and visual indicators (bounding boxes)

COCO-SSD: A pre-trained machine learning model capable of recognizing 90 different object classes

📦 Getting Started

Prerequisites

Ensure you have the following:

A modern web browser supporting the getUserMedia API (e.g., Chrome, Firefox)

Internet access to load the COCO-SSD model from a CDN

Running the Project

Clone the repository or download the project files.

Open index.html in a web browser.

Click the "Enable Webcam" button to start the live video feed.

Allow webcam access when prompted by your browser.

The application will automatically detect objects, displaying their names and confidence scores.

📁 Project Structure

├── index.html        # Webpage structure with script and style references
├── script.js         # JavaScript for webcam access, COCO-SSD model loading, and detection
└── styles.css        # CSS for styling the page and detection overlays

🔍 Code Overview

1. Webcam Access

Checks if the browser supports the getUserMedia API.

Enables webcam access upon clicking the "Enable Webcam" button.

2. Model Loading

The COCO-SSD model is loaded using cocoSsd.load().

The model is stored globally for efficient use during detection.

3. Real-Time Object Detection

predictWebcam() function detects objects in each webcam frame.

Objects with confidence scores greater than 66% are highlighted.

Draws bounding boxes and displays the object’s class name and confidence score.

4. Styling

Basic CSS styles for page layout.

Custom styles for the bounding boxes to highlight detected objects.

5. Error Handling

Displays a warning if webcam access is not supported.

Shows an alert if there is an error accessing the webcam.

📄 License

This project is licensed under the Apache License 2.0. See the LICENSE file for details.

📚 References

COCO-SSD Model Documentation

getUserMedia API Documentation

