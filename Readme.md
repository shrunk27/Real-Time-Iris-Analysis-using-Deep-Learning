# Iris Analysis with Deep Learning 👁️

A computer vision project that performs iris segmentation, color classification, and feature extraction using a combination of U-Net segmentation, CNNs, and classical image processing. This system captures images via webcam, detects eyes, extracts iris regions, analyzes iris patterns and color, and visualizes results interactively.

🚀 Features

U-Net based Iris Segmentation – Accurately segments iris regions from eye images.

Eye Detection – Uses dlib facial landmarks (with Haar cascade fallback).

Iris Color Classification – Hybrid approach with CNN + rule-based + feature-based methods.

Color Feature Extraction – Computes statistics in RGB, HSV, LAB, YUV color spaces.

Pattern & Texture Analysis – Extracts features like:

Crypts Density 🕳️

Furrows Prominence 🌀

Collarette Visibility 🎯

Pattern Complexity 🎨

Texture Contrast ⚡

Image Quality Assessment – Ensures reliable iris analysis using sharpness, contrast, and brightness checks.

Visualization Dashboard – Side-by-side plots of original images, segmented iris regions, color swatches, and feature comparisons.

📂 Project Structure
├── enhanced_iris_analysis.py   # Main script
├── models/                     # Pre-trained/temporary models
│   └── shape_predictor_68_face_landmarks.dat (required)
├── data/                       # Placeholder for captured/processed data
└── README.md                   # Project documentation

🛠️ Tech Stack

Languages: Python 3.x

Libraries:

Deep Learning: TensorFlow / Keras

Computer Vision: OpenCV, dlib

Machine Learning: scikit-learn

Visualization: matplotlib

Utilities: NumPy, Pandas, PIL

⚙️ Installation
1️⃣ Clone the repository
git clone https://github.com/shrunk27/Real-Time-Iris-Analysis-using-Deep-Learning
cd enhanced-iris-analysis

2️⃣ Create a virtual environment 
python -m venv venv
source venv/bin/activate   # On Mac/Linux
venv\Scripts\activate      # On Windows

3️⃣ Install dependencies
pip install -r requirements.txt

4️⃣ Download the facial landmark predictor

Download shape_predictor_68_face_landmarks.dat from dlib’s model zoo
.
Extract it into the models/ folder.

▶️ Usage

Run the script:

python enhanced_iris_analysis.py


The system will capture images via webcam.

It will analyze the left and right iris separately.

Results are displayed in a matplotlib visualization window with detailed statistics.

📊 Example Output
Left Eye:
  Color: Hazel (confidence: 0.78)
  Image Quality: 0.85
  Features:
    - Crypts Density: 0.03
    - Furrows Prominence: 2.15
    - Collarette Visibility: 0.51
    - Pattern Complexity: 0.85
    - Texture Contrast: 32.18

📌 Future Improvements

Train the CNN on a larger annotated iris dataset for higher accuracy.

Add real-time emotion + iris correlation analysis.

Build a Streamlit dashboard for interactive web-based results.

Deploy as a desktop/mobile app.

👩‍💻 Author

Shrunkhala S

🎓 Master’s in Business Intelligence & Analytics

🌍 Location: Ahmedabad, India

💼 Data Science | Computer Vision | Deep Learning

🔗 LinkedIn
 | GitHub