# Long Hair Detection System

An AI-powered application designed to analyze facial features to determine age and gender, with custom conditional logic to infer gender based on hair length for specific age groups.

## 📁 Repository Contents

* **`Long_Hair_Working.ipynb`**: The research notebook containing the feature engineering, model training, and performance evaluation for long/short hair classification.
* **`app.py`**: A Streamlit web application providing a deep-analysis interface for real-time face image processing.
* **`requirements.txt`**: A comprehensive list of dependencies and packages required to run the application.
* **`packages.txt`**: A list of packages to run the app on streamlit-hub

## 🚀 Features

* **AI Face Analysis**: Utilizes `MediaPipe` for landmark detection and `Segformer` for semantic hair parsing.
* **Conditional Gender Inference**: Implements custom logic where hair length overrides standard gender classification for individuals aged 20–30.
* **Age Estimation**: Provides estimated age based on grouped classification models.
* **Deep Analysis Pipeline**: Processes uploaded face images through multiple concurrent models to extract specific insights.

## 🔧 Setup & Installation

### 1. Prerequisites

Ensure you have Python 3.9+ installed. Clone this repository:

```bash
git clone https://github.com/KVAlwaysLearning/Long_Hair_Detection_Sub
cd Long_Hair_Detection_Sub

```

### 2. Install Requirements & Packages

The project relies on computer vision and deep learning frameworks. Install the necessary packages using:

```bash
pip install -r requirements.txt

```

**Key Dependencies included in `requirements.txt`:**

* `streamlit`: For the web user interface.
* `opencv-python`: For image processing and computer vision tasks.
* `torch` & `torchvision`: For deep learning model inference.
* `transformers`: For utilizing pre-trained `Segformer` models.
* `mediapipe`: For face detection and landmarker tasks.
* `gdown`: For managing and downloading large pre-trained model weights from Google Drive.
* `pillow`: For image manipulation.

### 3. Environment Setup

The application downloads necessary models from Google Drive upon first run. Ensure you have a stable internet connection for the initial initialization of the `Models/` directory.

## 💻 Usage

### Running the App

Launch the interactive web interface:

```bash
streamlit run app.py

```

### Exploring the Research

You can open `Long_Hair_Working.ipynb` in Jupyter, Google Colab, or VS Code to review the training methodology and how the hair-length-to-gender override logic was developed.

## 📂 Project Structure

```text
├── Models/            # Directory for downloaded pre-trained weights or custom trained weights (Refer .ipynb file)
├── app.py             # Streamlit application
├── Long_Hair_Working.ipynb # Research and training notebook
├── requirements.txt   # List of all Python dependencies
└── README.md          # Project documentation

```

## 🔗 Links

* **Live App**: [Long Hair Detection App](https://www.google.com/search?q=https://longhairdetection-app.streamlit.app/)
* **GitHub Repo**: [Long Hair Detection Repository](https://www.google.com/url?sa=E&source=gmail&q=https://github.com/KVAlwaysLearning/Long_Hair_Detection_Sub)

Visuals:
<img width="1223" height="604" alt="App_1" src="https://github.com/user-attachments/assets/76df7dd7-f53b-4f21-887d-c57c03abe6a7" />

<img width="1243" height="577" alt="App_2" src="https://github.com/user-attachments/assets/c746f484-e468-4936-b43f-3d16e97665d1" />

<img width="992" height="571" alt="App_3" src="https://github.com/user-attachments/assets/8aeff811-6259-4fb2-a71c-27d93adcd184" />

<img width="1154" height="583" alt="App_4" src="https://github.com/user-attachments/assets/6d74660f-6b32-4947-9a81-50303df4fcf8" />
