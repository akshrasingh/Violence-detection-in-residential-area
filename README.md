# VioGuard - Anomaly Detection for Violence Detection in Videos

VioGuard is an anomaly detection application designed to detect violent and non-violent frames in video clips. This application leverages a BiLSTM model, with MobileNetV2 as a spatio-temporal feature extractor, to accurately label frames in uploaded videos.

## Features
- Upload video clips for analysis.
- Receive processed videos with frame-wise labels indicating violence and non-violence.
- Utilizes state-of-the-art deep learning techniques for anomaly detection.

## Dataset
VioGuard is trained and tested on the 'Real Life Violence Situations Dataset' from Kaggle, which contains 800 MP4 files. The dataset includes:
- Violent clips featuring real street fights, with or without weapons (sticks, rods).
- Non-violent clips showing human activities such as sports, eating, and walking.

## Installation
1. Clone the repository:
    ```sh
    git clone https://github.com/Akshat-1729/Violence-detection-in-residential-area.git
    cd Violence-detection-in-residential-area
    ```

2. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

    **requirements.txt:**
    ```plaintext
    Flask
    Werkzeug
    tensorflow
    numpy
    opencv-python
    matplotlib
    simpleaudio
    ```

3. Ensure you have the necessary dataset in the appropriate directory.

## Usage
1. Navigate to the `app` directory:
    ```sh
    cd app
    ```
![image](https://github.com/user-attachments/assets/efed8779-259f-4e91-ab36-f11e2abc050b)


2. Run the application:
    ```sh
    python app.py
    ```

3. Open your web browser and go to `http://localhost:5000`.

4. Use the 'Upload Video' button to upload a video for processing.

5. Once the video is uploaded, the application will process it and return a video with frame-wise labels indicating violence and non-violence.


https://github.com/user-attachments/assets/47058a1e-4107-4289-b6e3-0593cfcddf3d



## Model
- **Feature Extractor**: MobileNetV2
- **Sequence Model**: BiLSTM
