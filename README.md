📸 Face Recognition Based Attendance System
This is a Flask-based Face Recognition Attendance System that uses OpenCV and machine learning (KNN classifier) to automate attendance tracking. It captures images from a webcam, identifies registered users using facial recognition, and marks their attendance with timestamped entries stored in CSV files.

🚀 Features
Face detection using Haar cascades (cv2.CascadeClassifier)        
Face recognition using K-Nearest Neighbors (KNN)
Real-time webcam interface for:
  Marking attendance
  Adding new users
Automatic training of the model when new users are added
Attendance logging in CSV format
Dashboard-style interface to:
  View today’s attendance
  Add/Delete users
Responsive frontend built using HTML + Bootstrap

🛠️ Technologies Used
Python (Flask, OpenCV, NumPy, Pandas, Joblib)
HTML5 + Bootstrap
Machine Learning (KNN Classifier from sklearn)
CSV-based lightweight database
