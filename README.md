# 📸 Face Recognition Based Attendance System

This is a **Flask-based Face Recognition Attendance System** that uses OpenCV and machine learning (KNN classifier) to automate attendance tracking. It captures images from a webcam, identifies registered users using facial recognition, and marks their attendance with timestamped entries stored in CSV files.

## 🚀 Features

- Face detection using Haar cascades (`cv2.CascadeClassifier`)
- Face recognition using K-Nearest Neighbors (KNN)
- Real-time webcam interface for:
  - Marking attendance
  - Adding new users
- Automatic training of the model when new users are added
- Attendance logging in CSV format
- Dashboard-style interface to:
  - View today’s attendance
  - Add/Delete users
- Responsive frontend built using **HTML + Bootstrap**

## 🛠️ Technologies Used

- Python (Flask, OpenCV, NumPy, Pandas, Joblib)
- HTML5 + Bootstrap
- Machine Learning (KNN Classifier from `sklearn`)
- CSV-based lightweight database

## 📁 Folder Structure

```
├── app.py                       # Main Flask application
├── templates/
│   └── home.html               # Frontend template
├── static/
│   └── faces/                  # Stores user face images
│   └── face_recognition_model.pkl  # Trained model
├── Attendance/
│   └── Attendance-<date>.csv   # Daily attendance logs
```

## 📸 How It Works

1. **Add New User**: Enter name and ID, then the system captures face samples via webcam.
2. **Train Model**: Automatically retrains the model with new data.
3. **Take Attendance**: Live face recognition identifies users and logs attendance.
4. **View Attendance**: See logged names, IDs, and timestamps on the dashboard.

## ✅ How to Run

```bash
git clone https://github.com/your-username/face-recognition-attendance.git
cd face-recognition-attendance
pip install -r requirements.txt
python app.py
```

Then, open your browser and go to `http://127.0.0.1:5000/`

## 📝 To-Do

- Improve model accuracy with more face data
- Add admin login and user authentication
- Export attendance reports to Excel or PDF
- Add cloud-based storage (Firebase, MongoDB, etc.)

## 🤝 Contributing

Feel free to fork this repository, make enhancements, and open pull requests!
