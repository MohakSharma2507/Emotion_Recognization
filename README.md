# Real-time Emotion Detection

This project utilizes OpenCV and DeepFace to perform real-time emotion recognition using your webcam. It detects faces in a video stream, analyzes facial expressions, and displays the dominant emotion on the screen.

## Features

- **Face Detection**: Uses OpenCV's Haar Cascade Classifier to detect faces in real-time.
- **Emotion Recognition**: Employs DeepFace to identify emotions such as happiness, sadness, anger, surprise, etc.
- **Real-time Processing**: Provides live video feed with emotion labels displayed on detected faces.

## Requirements

- Python 3.x
- OpenCV
- DeepFace

You can install the necessary libraries using the following commands:
```bash
pip install opencv-python
pip install deepface
```

## How to Run

1. Clone the repository and navigate to the project directory.

2. Run the script:
   ```bash
   python emotion_detection.py
   ```

3. A new window will open, showing the live video feed from your webcam. Detected faces will be highlighted with a bounding box, and the dominant emotion will be displayed above each face.

4. Press **'q'** to exit the application.

## Code Explanation

- **Face Detection**: The Haar Cascade Classifier from OpenCV detects faces within the video frame.
- **Emotion Analysis**: The detected face region is passed to DeepFace for emotion analysis.
- **Display**: The dominant emotion is labeled above the detected face on the video feed.

## Example Output

- A bounding box will appear around each detected face with the recognized emotion displayed above it.

## Troubleshooting

- Ensure your webcam is functioning properly.
- If the face detection or emotion recognition doesn't perform well, you may need to adjust parameters like `scaleFactor` and `minNeighbors` in the `detectMultiScale` method.
- For environments where GPU support is available, DeepFace will automatically leverage it if properly set up.

## Dependencies

```plaintext
- OpenCV: for real-time image processing.
- DeepFace: for emotion analysis on detected faces.
```



---

