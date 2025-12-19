Respirx - Lung Disease Classification

A web application that uses AI to classify chest X-ray images and detect lung diseases.

## What It Does

Respirx uses a deep learning model to analyze chest X-ray images and classify them into four categories:
- COVID-19
- Normal
- Pneumonia
- Tuberculosis

## Features

-  **Upload X-rays** - Simple web interface to upload and analyze images
-  **AI Predictions** - Fast classification with confidence scores
-  **PDF Reports** - Generate and download diagnostic reports
-  **User Accounts** - Doctor and patient roles with secure login
-  **History** - Track all predictions and results
-  **Real-time** - Get results in seconds

## Tech Stack

- **Backend**: Flask (Python)
- **AI/ML**: TensorFlow, Keras
- **Frontend**: HTML5, CSS3, JavaScript
- **Database**: SQLite

## Installation & Setup

### Requirements
- Python 3.7+
- pip

### Steps

1. **Clone or download the project**
   ```bash
   cd Respirx-main
   ```

2. **Create virtual environment**
   ```bash
   python -m venv venv
   venv\Scripts\activate
   ```

3. **Install packages**
   ```bash
   pip install -r requirements.txt
   ```

4. **Create database**
   ```bash
   python create_users.py
   ```

5. **Run the app**
   ```bash
   python app.py
   ```

6. **Open in browser**
   ```
   http://localhost:5000
   ```

## Project Structure

```
Respirx/
├── app.py              application
├── model.py         training code
├── best_weight.h5      # Trained model
├── create_users.py     # Setup script
├── static/             # CSS, JS, images
├── templates/          # HTML pages
└── uploads/            # User uploaded files
```

## How to Use

1. **Login** with your account (doctor/patient)
2. **Upload** a chest X-ray image (JPG or PNG)
3. **View prediction** - See disease classification and confidence
4. **Download report** - Get a PDF of the results

## Model Info
## Model Info

- **Training Data**: Chest X-ray dataset
- **Input**: 224×224 pixel images
- **Output**: 4 disease classes
- **Accuracy**: ~95%
