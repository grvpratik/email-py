# Email Spam Classifier

A Django-based web application that uses machine learning to classify emails as spam or ham (legitimate). This project implements a spam detection system with a user-friendly web interface.

## Features

- **Email Classification**: Analyze emails to determine if they are spam or legitimate
- **Machine Learning Model**: Uses trained models for accurate spam detection
- **Web Interface**: Clean and intuitive Django-based UI for easy interaction
- **Real-time Analysis**: Get instant results on email classification

## Project Structure

```
email-py/
├── models/                 # Machine learning model files
├── spam_classifier/        # Django app for spam classification
├── spam_project/          # Main Django project directory
├── template/              # HTML templates for the web interface
├── manage.py             # Django management script
├── requirements.txt      # Project dependencies
└── .gitignore           # Git ignore file
```

## Prerequisites

- Python 3.x
- pip (Python package manager)
- Virtual environment (recommended)

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/pratikgrv/email-py.git
   cd email-py
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python -m venv venv
   
   # On Windows
   venv\Scripts\activate
   
   # On macOS/Linux
   source venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run database migrations**
   ```bash
   python manage.py migrate
   ```

5. **Start the development server**
   ```bash
   python manage.py runserver
   ```

6. **Access the application**
   Open your web browser and navigate to `http://127.0.0.1:8000/`

## Usage

1. Navigate to the application in your web browser
2. Enter or paste the email text you want to analyze
3. Click the submit/analyze button
4. View the classification result (Spam or Ham)
5. The model will display the prediction along with confidence scores

## Technologies Used

- **Backend Framework**: Django
- **Machine Learning**: scikit-learn / TensorFlow (depending on model implementation)
- **Frontend**: HTML, CSS, JavaScript
- **Data Processing**: pandas, numpy
- **Natural Language Processing**: NLTK / spaCy (for text preprocessing)

## Model Information

The spam classifier uses machine learning algorithms trained on email datasets to identify patterns typical of spam emails, including:
- Suspicious keywords and phrases
- Email structure patterns
- Sender information patterns
- URL and link analysis
