# License Plate Detection and Recognition

This project uses **OpenCV** and **EasyOCR** to detect and recognize license plates from images and videos. It is optimized for **Google Colab**.

## Features

- Detect license plates in images/videos.
- Recognize text from license plates using **EasyOCR**.
- Real-time video processing and image upload support.

## Installation

To install the required libraries, run the following:

```bash
pip install opencv-python-headless easyocr imutils numpy matplotlib
For OpenCV system dependencies, run:
!apt-get update && apt-get install -y libgl1-mesa-glx
##Usage
##Image Detection
image = cv2.imread('path_to_image.jpg')
processed_image, plate_text, plate_region = process_image(image)
print("Detected License Plate Text:", plate_text)
##Video Detection
process_video()
##Functions Overview
detect_plate(image): Detects the license plate region in an image.

recognize_plate_text(image, location): Recognizes and extracts text from the detected plate region.

process_image(image): Detects the plate and extracts text from it in a single image.

process_video(video_path): Detects and recognizes plates in each frame of a video file.
##License
This project is licensed under the MIT License. See the LICENSE file for details.


