# Football Object Detection and Tactical Analysis

A comprehensive solution for football/soccer video analysis and tactical planning, combining object detection for player/field tracking and an interactive tactical board for strategy visualization.

## 🌟 Features

### Object Detection
- Player detection and tracking using YOLOv8L
- Field keypoint detection using YOLOv8M
- Real-time video analysis capabilities

### Interactive Tactical Board
- Multiple formation presets:
  - 4-3-3 (Attacking/Defensive)
  - 4-4-2 (Diamond/Flat)
  - 3-5-2
  - 3-4-3
  - 5-3-2
  - 4-2-3-1
- Player role customization with detailed descriptions:
  - Ball-playing Defender
  - Deep-lying Playmaker
  - And more...
- Tactical style templates:
  - Tiki-taka
  - Counter-attack
  - Gegenpressing


## 📋 Requirements

The project requires Python 3.8+ and the following main dependencies:
- ultralytics
- streamlit
- streamlit-drawable-canvas
- opencv-python
- Pillow
- numpy

For a complete list of dependencies, see `requirements.txt` or `environment.yml`.

## 🚀 Installation

1. Clone the repository:
```bash
git clone https://github.com/gokul-s05/football_analytics.git
cd football-object-detection
```

2. Create and activate a virtual environment:
```bash
# Using conda
conda env create -f environment.yml
conda activate football-detection

# OR using pip
python -m venv .venv
source .venv/bin/activate  # Linux/Mac
.venv\Scripts\activate     # Windows
pip install -r requirements.txt
```

## 💻 Usage

### Object Detection

1. Place your video file in the project directory
2. Run the detection notebook:
```bash
jupyter notebook "Football Object Detection With Tactical Map.ipynb"
```

### Tactical Board Web App

1. Navigate to the Streamlit web app directory:
```bash
cd "Streamlit web app/outputs"
```

2. Launch the web application:
```bash
python -m streamlit run app.py
```

3. Access the application in your browser at `http://localhost:8501`

## 📁 Project Structure

```
Football object detection/
├── models/                          # Trained model weights
│   ├── Yolo8L Players/             # Player detection model
│   └── Yolo8M Field Keypoints/     # Field keypoint detection model
├── Streamlit web app/              # Interactive web application
│   └── outputs/                    # Web app components and resources
├── config pitch dataset.yaml       # Field detection configuration
├── config players dataset.yaml     # Player detection configuration
├── environment.yml                 # Conda environment specification
└── requirements.txt                # Pip dependencies
```
[Watch the Video] (https://drive.google.com/file/d/1uCeN0S8DZUBXREr_46xpKAZZXj-084d9/view?usp=sharing)
## 🎯 Model Information

- Player Detection: YOLOv8L model trained for football player detection
- Field Keypoint Detection: YOLOv8M model trained for field landmark detection
- Pre-trained weights are included in the `models/` directory

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
