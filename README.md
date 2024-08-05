# Face, Eye, and Smile Detection

This project demonstrates real-time detection of faces, smiles, and eyes using OpenCV. It captures video from your webcam, processes each frame to detect and annotate faces, smiles, and eyes, and displays the result in a window.

## Features

- **Face Detection**: Identifies and highlights faces in the video feed.
- **Smile Detection**: Detects and highlights smiles within detected faces.
- **Real-Time Processing**: Provides real-time video processing and display.

## Requirements

- **Python**: Make sure Python is installed on your system.
- **OpenCV**: Required for image processing and computer vision tasks.

Install the required package using pip:

```bash
pip install opencv-python-headless

```

## Setup

1. **Clone the Repository**:

```bash
Copy code
git clone <repository-url>
cd <repository-directory>
```

2. **Download Haar Cascade Files**:

- Download the Haar Cascade XML files for face, smile detection from OpenCV's GitHub repository.
- Place the downloaded files in a directory named data:
  - haarcascade_frontalface_default.xml
  - haarcascade_smile.xml

3. **Run the Script**:

```bash
Copy code
python <script-name>.py
```

Replace <script-name> with the name of your Python script file.

## Usage:

- A window will open displaying the video feed from your webcam with detected faces and smiles.
- Press q to exit the video feed and close the application.

## How It Works

1. **Initialization**:

Loads Haar Cascade classifiers for face and smile detection.
Initializes video capture from the webcam.

2. **Detection**:

- Converts each video frame to grayscale.
- Detects faces in the grayscale image.
- For each detected face, detects smiles and draws rectangles around them.
- Displays the processed video frame with annotations.

3. **Exit**:

- Press q or close the window to stop the video feed and terminate the application.

## Troubleshooting

- **No Video Display**: Ensure your webcam is properly connected and accessible. Verify that OpenCV is correctly installed.
- **Detection Issues**: Ensure the Haar Cascade XML files are correctly placed in the data directory and that they are correctly loaded.

## Customization

- **Detection Parameters**: Adjust detection sensitivity by modifying parameters in the detect function.
- **Additional Features**: Extend functionality to include features like eye detection or emotion recognition.

## License

This project is open-source and available under the MIT License. You are free to use, modify, and distribute the code according to the terms of the license.

## Contact

For any questions or feedback, please refer to the contact details provided in the repository.
