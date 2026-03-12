# 🩺 CliniScan – AI Lung Abnormality Detection

CliniScan is a deep learning-based medical imaging system that detects lung abnormalities from Chest X-ray images.
The project uses the YOLOv8 object detection model and provides an easy-to-use Streamlit web interface for uploading and analyzing X-ray images.

This project was developed as part of a Virtual Internship at Infosys.

🚀 Features

 - Detects multiple lung abnormalities from chest X-ray images

 - Uses Ultralytics YOLOv8 for fast and accurate object detection

 - Built with PyTorch deep learning framework

 - Interactive web interface using Streamlit

 - GPU-supported training for faster model development

🛠️ Technologies Used

 - Python
 - PyTorch
 - Ultralytics YOLOv8
 - Streamlit
 - NumPy
 - Pandas

 📂 Project Structure
 
 CliniScan
 │
 ├── data
 │   ├── raw
 │   └── processed
 │
├── src
│   ├── 1_preprocess_annotations.py
│   ├── 2_split_data.py
│   ├── 4_train_yolo.py
│   └── streamlit_app.py
│
├── weights
│   └── best.pt
│
├── requirements.txt
└── README.md
⚙️ Installation

Clone the repository:

git clone https://github.com/YOUR_USERNAME/CliniScan-AI-Lung-Abnormality-Detection.git
cd CliniScan-AI-Lung-Abnormality-Detection

Create virtual environment:  python -m venv .venv

Activate environment: 

Windows

.venv\Scripts\activate

Install dependencies:

pip install -r requirements.txt

📊 Dataset

This project uses the VinBigData Chest X-ray Dataset.

Due to the large dataset size, the images and annotations are not included in this repository.

🏋️ Model Training

Run the preprocessing scripts:

python src/1_preprocess_annotations.py

Split the dataset:

python src/2_split_data.py

Train the model:

python src/4_train_yolo.py

After training, the model weights will be saved as:

runs/detect/train/weights/best.pt

Move the file to the weights folder.

💻 Run the Application

Start the Streamlit app:

streamlit run src/streamlit_app.py

Then open the application in your browser and upload a Chest X-ray image to detect abnormalities.

📌 Disclaimer

This project is intended for educational and research purposes only.
It is not a substitute for professional medical diagnosis.

If you want, I can also give you a better version with GitHub badges and demo screenshots so your repo looks much more impressive for internships and placements.
