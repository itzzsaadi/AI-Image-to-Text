# AI-Image-to-Text
AI-powered web app that extracts text from images, corrects grammar, and detects toxic language using OCR, NLP, and Machine Learning.


# 🧠 AI Text Extractor & Toxicity Classifier

This project is a full-stack AI application that extracts text from uploaded images using OCR (Optical Character Recognition), corrects grammar using an NLP model, and classifies the content based on toxicity categories using a trained machine learning model.

### 🚀 Key Features

- 📷 **OCR Text Extraction**: Uses Tesseract to extract high-confidence words from images.
- 🧼 **Text Cleaning & Enhancement**: Removes noise, fixes grammar using a T5 transformer model.
- 🧠 **Toxicity Classification**: Detects multiple types of toxic content using a LinearSVC model.
- 🌐 **User-Friendly Web Interface**: Built with Flask and Bootstrap for uploading and previewing images.
- 🧪 **Live Preview & Confidence Filtering**: Only processes sharp images with confidence score > 70.
- 🧰 **Blurry Image Detection**: Enhances blurry images with automatic filtering.
- 🌍 **Deployed via Ngrok**: Easily shareable temporary public URL.

### 🧰 Technologies Used

- Python, Flask, Bootstrap (Frontend)
- PyTesseract (OCR), OpenCV, Pillow (Image Processing)
- scikit-learn (ML), transformers (NLP)
- Joblib (Model Saving), Ngrok (Public URL Hosting)

### 📁 Files

- `app.py`: Flask backend for image upload and model inference.
- `model.pkl`, `tfidf_vectorizer.pkl`: Pre-trained SVM model and TF-IDF vectorizer.
- `templates`: Contains the HTML for the UI.
- `train.csv`: Training data for the toxicity classifier.

### 🏁 How to Run

1. Clone the repo.
2. Install dependencies:
    pip install -r requirements.txt
3. Add your Ngrok Auth Token in the script.
4. Run the Flask app.
   python app.py
5. Open the printed Ngrok URL in your browser.

**Requirements**
Python 3.7+
Tesseract OCR
Ngrok (for sharing locally hosted app)

**Future Improvements**
Save and export results
Add language selection for multilingual OCR
Improve UI responsiveness
Enable multiple image uploads
