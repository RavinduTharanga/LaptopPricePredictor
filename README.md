
Laptop Price Predictor
======================

This is a web application that predicts laptop prices based on specifications like RAM, weight, CPU, GPU, and more. Built using Flask, this app loads a pre-trained machine learning model to make predictions on the fly.

Features
--------
- User-friendly web interface to input laptop specifications
- Real-time price prediction using a trained ML model
- Deployed using Gunicorn and Procfile (suitable for Heroku or similar platforms)

Tech Stack
----------
- Backend: Python, Flask
- Machine Learning: scikit-learn, joblib, NumPy
- Deployment: Gunicorn
- Web Templating: Jinja2, HTML

Project Structure
-----------------
app.py                # Main application file
requirements.txt      # Python dependencies
Procfile              # For deployment
templates/
    index.html        # HTML frontend (must be added)
model/
    predictor.pickle  # Trained ML model (must be added)

Setup Instructions
------------------
1. Clone the repository:
   git clone https://github.com/yourusername/laptop-price-predictor.git
   cd laptop-price-predictor

2. Create a virtual environment and activate it:
   python -m venv venv
   source venv/bin/activate   (On Windows: venv\Scripts\activate)

3. Install dependencies:
   pip install -r requirements.txt

4. Make sure the model/predictor.pickle file exists.

5. Run the application:
   python app.py

Deployment
----------
Use gunicorn for production deployment:
   gunicorn app:app

License
-------
This project is licensed under the MIT License.
