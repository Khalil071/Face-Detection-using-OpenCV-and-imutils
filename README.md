Face Detection using OpenCV and imutils

Overview

This project implements face detection in images using OpenCV's cv2 module along with the imutils library for image processing. The model detects faces in images and highlights them with bounding boxes.

Technologies Used

OpenCV (cv2): Provides pre-trained face detection models (Haar cascades & DNN models).

imutils: Simplifies image transformations such as resizing and rotation.

Project Structure

├── dataset/                     # Contains images for face detection
├── models/                      # Pre-trained face detection models
├── notebooks/                   # Jupyter notebooks for experimentation
├── src/                         # Source code
│   ├── face_detector.py         # Face detection implementation
│   ├── preprocess.py            # Image preprocessing functions
│   ├── evaluate.py              # Model evaluation script
├── requirements.txt             # Required dependencies
├── README.md                    # Project documentation

Installation

Clone the repository:

git clone https://github.com/your-username/face-detection-opencv.git
cd face-detection-opencv

Create a virtual environment (optional but recommended):

python -m venv env
source env/bin/activate  # On Windows use: env\Scripts\activate

Install dependencies:

pip install -r requirements.txt

Face Detection Usage

Run the face detection script:

python src/face_detector.py --image_path path/to/image.jpg

This will display the image with detected faces highlighted.

Face Detection Model Options

The script supports:

Haar cascades: A lightweight, fast model for face detection.

Deep Learning-based models (DNNs): More accurate but computationally expensive.

You can switch between these models in face_detector.py.

Evaluation

Run the evaluation script to test accuracy on a dataset:

python src/evaluate.py --dataset dataset/

Future Improvements

Implement real-time face detection using a webcam.

Integrate facial landmark detection for enhanced accuracy.

Optimize detection speed using multi-threading.

Contributing

Feel free to contribute by opening issues or submitting pull requests!

License

This project is licensed under the MIT License.
