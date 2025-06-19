# Flask Cloud Deployment Boilerplate
Created by Jeya Kirushna  

🚀 A ready-to-deploy Flask app for Google Cloud Platform (GCP) services like App Engine & Cloud Run

## 📌 Features

✅ Minimal Flask app with two endpoints:  
- `/` → Returns "Hello World!"  
- `/echo/<name>` → Returns JSON response  

✅ Pre-configured for GCP deployments:  
- `app.yaml` → Google App Engine (Standard)  
- `Dockerfile` → Cloud Run / Kubernetes / App Engine Flexible  
- `cloudbuild.yaml` → CI/CD with Google Cloud Build  

✅ Production-ready with:  
- Gunicorn WSGI server  
- Proper dependency pinning  
- Optimized Docker image  

## ⚡ Quick Deploy

### 1. Google App Engine (Standard)
```sh
gcloud app deploy

gcloud builds submit --tag gcr.io/YOUR-PROJECT-ID/flask-app  
gcloud run deploy --image gcr.io/YOUR-PROJECT-ID/flask-app --platform managed
```
### 1. Google App Engine (Standard)
```python -m venv venv  
source venv/bin/activate  # On Windows: venv\Scripts\activate  
pip install -r requirements.txt  
flask run  # Runs at http://localhost:5000
```
### 📂 Project Structure
```
├── main.py             # Flask application  
├── requirements.txt    # Python dependencies (pinned versions)  
├── app.yaml            # App Engine config  
├── cloudbuild.yaml     # CI/CD pipeline for GCP  
├── Dockerfile          # Production container setup  
└── README.md
```

📞 Contact & Support  
🔗 Let's connect! → Jeya Kirushna on LinkedIn: https://www.linkedin.com/in/jeyakirushna/  
💡 Need cloud hosting help? Feel free to reach out for consulting!
