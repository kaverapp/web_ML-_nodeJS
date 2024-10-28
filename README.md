Real-Time Object Detection with COCO-SSD



This project demonstrates real-time object detection using the COCO-SSD model in a web application. It utilizes JavaScript, HTML, and CSS to access the user's webcam, detect objects in the camera's view, and highlight them with bounding boxes and confidence scores.

Features
Uses the COCO-SSD machine learning model for object detection.
Real-time webcam stream processing.
Displays detected objects along with their confidence scores.
Highlights objects in the live video feed with bounding boxes.
Technologies Used
JavaScript: For implementing the logic for webcam access, COCO-SSD model loading, and object detection.
HTML: For structuring the webpage and including necessary elements like buttons and the video stream.
CSS: For basic styling and visual indicators (e.g., highlighter for detected objects).
COCO-SSD: A pre-trained machine learning model for object detection, which can recognize 90 different object classes.
Getting Started
Prerequisites
Ensure you have the following:

A modern web browser that supports the getUserMedia API for webcam access (e.g., Chrome, Firefox).
Internet access to load the COCO-SSD model from a CDN.
Running the Project
Clone the repository or download the project files.

Open the index.html file in a web browser.

Click on the "Enable Webcam" button to start the live video feed. If prompted, allow the browser to access the webcam.

The application will automatically start detecting objects in the webcam feed, displaying their names and confidence scores.

Project Structure
index.html: Contains the structure of the web page and includes the necessary script and style tags.
script.js: Contains the JavaScript code for accessing the webcam, loading the COCO-SSD model, and handling real-time object detection.
styles.css: Contains the CSS styles for the page, including styles for the live view and highlighter elements.
Code Overview
Webcam Access
The application checks if the browser supports the getUserMedia API. If supported, it enables webcam access when the user clicks the "Enable Webcam" button.

Model Loading
The COCO-SSD model is loaded using the cocoSsd.load() method. The model is stored globally for use in the object detection function.

Real-Time Object Detection
The predictWebcam() function is responsible for detecting objects in each frame of the webcam stream.
Detected objects with a confidence score greater than 66% are highlighted in the live video feed.
Each detected object's bounding box is drawn, and its class name and confidence score are displayed.
Styling
Basic CSS is used to style the elements on the page, including the highlighter box for detected objects.

Error Handling
If the browser does not support webcam access, a warning is displayed.
If there is an error accessing the webcam, an alert is shown to the user.
License
This project is licensed under the Apache License 2.0 - see the LICENSE file for details.

References
COCO-SSD Model Documentation
getUserMedia API Documentation
