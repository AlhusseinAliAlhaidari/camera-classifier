# 📷 Camera Classifier v0.1 Alpha

A simple, interactive computer vision application built with Python. This tool allows you to use your webcam to capture images for two distinct classes, train a machine learning model on the fly, and perform real-time image classification.

## ✨ Features
- **Live Camera Feed**: View your webcam feed directly inside the app.
- **Custom Classes**: Define your own class names dynamically (e.g., "Person" vs. "Empty", or "Apple" vs. "Orange").
- **Interactive Dataset Collection**: Capture training images for each class with a single click.
- **On-the-Fly Training**: Train the classifier instantly based on the collected frames.
- **Real-Time Prediction**: Toggle auto-prediction to see the model classify the live feed in real-time.
- **Docker Support**: Pre-configured `Dockerfile` and `docker-compose.yml` for containerized environments.

## 🛠️ Technologies Used
- **Python 3**
- **Tkinter**: For the Graphical User Interface (GUI).
- **OpenCV (`cv2`)**: For capturing and processing webcam frames.
- **Pillow (`PIL`)**: For image manipulation within the Tkinter UI.
- **Machine Learning**: Custom classification model (`model.py`).

## 🚀 How to Run Locally

### Prerequisites
Make sure you have Python installed, then install the required dependencies:
```bash
pip install -r requirements.txt
```
*(Note: You will also need OpenCV and Pillow installed `pip install opencv-python pillow scikit-learn numpy` depending on your `model.py` requirements).*

### Running the App
Navigate to the source folder and run the `main.py` file:
```bash
cd camera-classifier
python main.py
```

## 🐳 Running with Docker
If you prefer using Docker, you can build and run the application using Docker Compose:

```bash
docker-compose up --build
```
*(Note: Running GUI applications inside Docker might require additional X11 server forwarding configuration depending on your host OS).*

## 💡 How to Use
1. Upon running the app, you will be prompted to enter the names of **Class 1** and **Class 2**.
2. Position an object in front of the camera and click the button for **Class 1** multiple times to save training images.
3. Place a different object and click the button for **Class 2** multiple times.
4. Click **Train Model**.
5. Click **Predict** for a single prediction, or click **Auto Prediction** for a continuous real-time classification.
6. Use **Reset** to clear the saved images and start over.

## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

---
*Created by [AlhusseinAliAlhaidari](https://github.com/AlhusseinAliAlhaidari)*
