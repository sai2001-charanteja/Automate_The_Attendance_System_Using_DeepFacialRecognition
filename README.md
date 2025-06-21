Presentation of this Project:
https://docs.google.com/presentation/d/1d9BbBote9bxQ8ogcSs__dbhzmKTu7oAB33O06LdY0A0/edit?usp=sharing

🎓 Automate Attendance System with Deep Facial Recognition

A final-year B.Tech project that automates the traditional attendance system using deep learning and computer vision techniques. This Python-based solution leverages facial recognition to mark student attendance in real-time, minimizing manual effort and eliminating proxy issues.

📌 Table of Contents

Overview

Features

Tech Stack

Folder Structure

Installation

Usage

Results


🚀 Overview
	Traditional attendance systems are tedious and susceptible to manipulation. This project proposes an intelligent system that captures classroom video, detects and recognizes student faces using deep learning, and marks attendance automatically based on attentiveness across frames.

The system also sends attendance reports to students and administrators via email and WhatsApp, ensuring transparency and accessibility.

🌟 Features

	🎥 Video capture and frame sampling

	🧠 Deep learning-based multi-face detection

	🧾 Face recognition using pre-trained VGG-Face model

	📊 Attendance tracking based on frame-wise attentiveness

	📩 Automated report generation and notifications via:

		Email (RedMail)

		WhatsApp (Twilio)

	✅ Accuracy: 99.38% on the LFW benchmark dataset

🛠️ Tech Stack

	Language: Python 3.7+

Libraries:

	OpenCV, Dlib
	TensorFlow + Keras
	Pandas, NumPy, Matplotlib
	RedMail (Email)
	Twilio (WhatsApp)
	Model: VGG-Face CNN
	Deployment: Google Colab

📁 Folder Structure

	Face_Recognition/
	├── Images/                  # Training images (10 per student)
	├── Images_crop/             # Cropped face images
	├── Test_Images/             # Test images from video
	├── Test_Images_crop/        # Cropped test images
	├── StudentAttendance/       # Excel files with attendance logs
	├── Predictions/             # Annotated predicted images
	├── Students_Info.xlsx       # Student details with email & phone
	└── face_classifier_model.h5 # Trained classifier model
	🖥️ Installation

Run in Google Colab or local Jupyter Notebook.

🔐 Configure Twilio & Outlook credentials in SendMessage() and sendmail() functions.

🧪 Usage
Train the Model
Run the script to:

	Crop and embed faces using VGG-Face
	Train a Softmax classifier on embeddings
	Test with a Video
	Upload a class recording
	Extract frames every 1000ms
	Detect and recognize faces
	Calculate frame-wise attentiveness
	Generate Attendance
	Create Excel attendance logs
	Send individual emails and WhatsApp messages to students

📊 Results

	📸 Total students trained: 7
	🎯 Model accuracy: 99.38%
	✔️ Real-time detection & recognition
	📧 Notifications sent with dynamic HTML emails

Sample output includes:

Cropped and predicted student face images

![19SS1A0507](https://github.com/user-attachments/assets/3ca3e834-158a-4bcd-8c67-8d9e07ee2cdf)

Attendance spreadsheet with attentiveness scores

![Screenshot (14)](https://github.com/user-attachments/assets/bc7afe03-baa0-4e52-b095-bbb6d33d4fd8)


Personalized feedback via WhatsApp & email

![Screenshot (15)](https://github.com/user-attachments/assets/301429c1-3b02-4be2-bb29-f77504b006d7)

![IMG_20230613_132856](https://github.com/user-attachments/assets/6196f51d-0227-43bc-8289-0f36b807789d)

