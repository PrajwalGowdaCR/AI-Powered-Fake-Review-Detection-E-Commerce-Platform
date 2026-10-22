# Fake Review Detection - Backend API

Flask-based REST API for detecting fake reviews using machine learning.

## 🚀 Features

- Machine learning model for fake review detection
- TF-IDF vectorization for text processing
- REST API endpoints for predictions
- NLTK-based text preprocessing

## 📋 Prerequisites

- Python 3.8+
- pip

## 🛠️ Installation

1. Clone the repository:
```bash
git clone https://github.com/hitesh-patgar/fake-review-backend.git
cd fake-review-backend
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Download NLTK data (if needed):
```python
python -c "import nltk; nltk.download('stopwords')"
```

## 🏃 Running Locally

```bash
python backend_api.py
```

The API will be available at `http://localhost:5000`

## 📡 API Endpoints

### POST /predict
Predict if a review is fake or genuine.

**Request:**
```json
{
  "review": "This product is amazing! Best purchase ever!"
}
```

**Response:**
```json
{
  "label": "genuine"
}
```

### POST /detect-fake-review
Enhanced endpoint with additional metadata.

**Request:**
```json
{
  "review": "This product is amazing! Best purchase ever!"
}
```

**Response:**
```json
{
  "label": "genuine",
  "is_fake": false
}
```

## 🚢 Deployment

### Render

1. Create a new Web Service on Render
2. Connect your GitHub repository
3. Set build command: `pip install -r requirements.txt`
4. Set start command: `gunicorn backend_api:app`
5. Deploy!

## 📁 Project Structure

```
fake-review-backend/
├── backend_api.py           # Main Flask application
├── fake_review_model.pkl    # Trained ML model
├── tfidf_vectorizer.pkl     # TF-IDF vectorizer
├── requirements.txt         # Python dependencies
├── Procfile                 # Render deployment config
└── .gitignore              # Git ignore rules
```

## 🔒 Security

- Never commit `.env` files
- Keep model files secure
- Use environment variables for sensitive data

## 📝 License

MIT License
