# Colab-PoseNet-RealTime

## Overview
This project demonstrates real-time human pose detection using **MediaPipe** and a custom **Convolutional Neural Network (CNN)** model. It is designed to run directly in **Google Colab**, where it utilizes the webcam for live pose detection and classification. The main objective of this repository is to provide a pipeline that captures real-time webcam data, processes it with MediaPipe to extract pose landmarks, and classifies the detected pose using a CNN model.

## Features
- **Real-time Pose Detection**: Utilizes MediaPipe for efficient pose detection.
- **Custom CNN Model**: Built for classifying human poses using key pose landmarks.
- **Webcam Support in Colab**: Leverages JavaScript to access the webcam inside the Colab environment.
- **Simple and Customizable**: The CNN model and the pipeline are easy to customize for your specific use case or dataset.

## How It Works
1. The **MediaPipe** library is used for detecting human pose landmarks from a live webcam feed.
2. These landmarks (x, y, z coordinates for 33 body points) are preprocessed and passed into a simple CNN model for classification.
3. The project uses JavaScript to capture webcam data within Colab and processes it in real-time.
4. The processed images, along with the predicted pose class, are displayed in the Colab output.

## How to Run
Follow these steps to run the project in Google Colab:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/RahmaniSajjad/Colab-PoseNet-RealTime.git
   cd Colab-PoseNet-RealTime
   ```

2. **Open in Google Colab**: 
   Upload the `Colab-PoseNet-RealTime.ipynb` file from this repository to your Google Drive and open it with Google Colab.

3. **Install dependencies**:
   In the Colab notebook, run the following code to install the required packages:
   ```python
   !pip install mediapipe opencv-python tensorflow
   ```

4. **Run the notebook**:
   Execute the cells in the notebook. It will automatically capture webcam images and start detecting and classifying poses.

5. **Enable Webcam Access**:
   When prompted, allow the notebook to access your webcam for real-time detection.

## Files
- **Colab-PoseNet-RealTime.ipynb**: Main notebook containing the code for real-time pose detection and classification.

## Usage
To customize the project:
- Modify the CNN architecture in the `build_cnn_model()` function to suit your application.
- Train the CNN on a different dataset if you want to classify custom poses.
- Adjust the number of pose classes by modifying the output layer of the CNN model.

## Requirements
- **Python 3.x**
- **Google Colab** (for webcam support)
- **Libraries**: 
  - `mediapipe`
  - `opencv-python`
  - `tensorflow`

## Contributing
Feel free to open issues or submit pull requests if you have suggestions or improvements.

## Author
[Sajjad Rahmani](https://github.com/RahmaniSajjad)

## License
This project is licensed under the MIT License.
