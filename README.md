# Motion Detection System

![Motion Detection](https://img.shields.io/badge/Motion-Detection-blue)
![Python](https://img.shields.io/badge/Python-3.x-green)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-orange)

A real-time motion detection system built with Python and OpenCV that can detect and track moving objects in video streams. This project is particularly effective for surveillance, security systems, and activity monitoring applications.

## 🚀 Features

- **Real-time Processing**: Instant detection and tracking of moving objects
- **Smart Object Detection**: 
  - Configurable sensitivity levels
  - Noise reduction through Gaussian blur
  - Intelligent contour detection
- **Visual Feedback**:
  - Bounding boxes around detected motion
  - Real-time status display
  - Movement indicators
- **Video Processing**:
  - Support for multiple video formats
  - Customizable output resolution
  - Frame-by-frame analysis
  - Video recording capabilities

## 📋 Prerequisites

- Python 3.x
- OpenCV (cv2)
- NumPy
- Jupyter Notebook (for running the demo)

## 🛠️ Installation

1. Clone the repository:
```bash
git clone https://github.com/Yossefmohammed/Motion-detection.git
cd Motion-detection
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

## 💻 Usage

1. Launch Jupyter Notebook:
```bash
jupyter notebook
```

2. Open `emotion detection_computer_vision.ipynb`

3. Update the video source path:
```python
cap = cv.VideoCapture("path_to_your_video.mp4")
```

4. Run the cells to start motion detection

### Output
- Real-time video display with motion detection
- Saved output video as 'testing.avi'
- Resolution: 1280x720
- Frame rate: 30 FPS

## 🔧 Technical Details

### Motion Detection Algorithm
1. **Frame Capture**: Captures consecutive frames from video source
2. **Frame Difference**: Computes absolute difference between frames
3. **Preprocessing**:
   - Grayscale conversion
   - Gaussian blur application (5x5 kernel)
4. **Motion Detection**:
   - Thresholding (threshold: 60)
   - Dilation (iterations: 10)
   - Contour detection
5. **Object Tracking**:
   - Contour area filtering (min: 900 pixels)
   - Bounding box generation
   - Status display

### Key Parameters
- Threshold Value: 60
- Minimum Contour Area: 900 pixels
- Output Resolution: 1280x720
- Frame Rate: 30 FPS
- Gaussian Blur Kernel: 5x5

## 📝 Project Structure
```
Motion-detection/
├── emotion detection_computer_vision.ipynb  # Main implementation
├── background video   people   walking.mp4  # Sample video
├── emotions detections.mp4                 # Sample video
├── vtest.avi                              # Test video
└── README.md                              # Documentation
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📧 Contact

Youssef - [ypssefmohammedahmed@gmail.com]
Project Link: [https://github.com/Yossefmohammed/Motion-detection](https://github.com/Yossefmohammed/Motion-detection)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- OpenCV community for the excellent computer vision library
- Python community for the amazing programming language
- All contributors who have helped improve this project
