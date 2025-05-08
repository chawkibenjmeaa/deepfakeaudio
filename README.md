# 🎙️ Deepfake Audio Detection with AI

An end-to-end system for detecting deepfake audio using machine learning. The project features two models: a baseline model achieving 88% accuracy and an advanced model reaching 93% accuracy. Built with Django for the backend and a user-friendly web interface for audio analysis.


## 📌 Table of Contents

* [Project Overview](#project-overview)
* [Features](#features)
* [Tech Stack](#tech-stack)
* [Dataset](#dataset)
* [Machine Learning Models](#machine-learning-models)
* [Web Application](#web-application)
* [Steganography Tools](#steganography-tools)
* [Installation](#installation)
* [Usage](#usage)
* [License](#license)

## 🧠 Project Overview

This project aims to detect deepfake audio clips using machine learning techniques. It provides a web interface for users to upload audio files and receive analysis results indicating the likelihood of the audio being a deepfake.

## ✨ Features

* **Deepfake Detection**: Analyze audio files to determine authenticity.
* **Two Models**:

  * *Baseline Model*: Achieves 88% accuracy.
  * *Advanced Model*: Achieves 93% accuracy.
* **Web Interface**: User-friendly platform for uploading and analyzing audio files.
* **Steganography Tools**: Embed and extract hidden messages within audio files.

## 🛠️ Tech Stack

* **Backend**: Django
* **Machine Learning**: Keras, TensorFlow
* **Frontend**: HTML, CSS, JavaScript
* **Database**: SQLite
* **Others**: NumPy, Pandas, LibROSA

## 🎧 Dataset

The models are trained on a curated dataset comprising both genuine and deepfake audio samples. The dataset includes various speakers and scenarios to ensure model robustness.

*Note: Due to licensing restrictions, the dataset is not included in this repository.*

## 🤖 Machine Learning Models

Two models are developed for deepfake audio detection:

1. **Baseline Model**:

   * Architecture: Convolutional Neural Network (CNN)
   * Accuracy: 88%
   * File: `deepfakedetection.keras`

2. **Advanced Model**:

   * Architecture: Enhanced CNN with additional layers and regularization
   * Accuracy: 93%
   * File: `deepfakedetectioncyber.keras`

## 🌐 Web Application

The Django-based web application allows users to:

* Upload audio files for analysis.
* View results indicating the probability of the audio being a deepfake.
* Access steganography tools for embedding and extracting hidden messages.

## 🔐 Steganography Tools

Located in the `steganoapp/` directory, these tools enable:

* **Embedding**:

  ```bash
  python steganoapp/embed.py --input audio.wav --output stego_audio.wav --data secret.txt
  ```

* **Extraction**:

  ```bash
  python steganoapp/extract.py --input stego_audio.wav --output extracted.txt
  ```

## 🚀 Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/chawkibenjmeaa/deepfakeaudio.git
   cd deepfakeaudio
   ```

2. **Create and activate a virtual environment**:

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Apply migrations**:

   ```bash
   python manage.py migrate
   ```

5. **Run the development server**:

   ```bash
   python manage.py runserver
   ```

## 📈 Usage

1. Open your web browser and navigate to `http://127.0.0.1:8000/`.
2. Upload an audio file using the provided interface.
3. View the analysis results indicating the likelihood of the audio being a deepfake.
4. Utilize steganography tools as needed.

## 📄 License

This project is licensed under the MIT License.


