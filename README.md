# Real-Time YOLO Object Detection on Google Colab 🎥

A hybrid Python/JavaScript notebook that performs real-time object detection using your webcam and YOLOv8 inside **Google Colab**. Designed to bypass Colab's streaming bottlenecks, this system delivers smooth, high-FPS performance by offloading rendering to the browser and transferring only lightweight detection JSON.

## 🚀 Features

- Real-time webcam streaming inside Colab
- YOLOv8 powered by Ultralytics (supports `yolov8n.pt` or custom models)
- HTML Canvas rendering with:
  - Bounding boxes & class labels
  - Confidence scores
  - FPS & inference time
  - Frame counter
- Auto-detects CPU/GPU (CUDA) without code changes
- Low-bandwidth architecture (JPEG frames → JSON detections)
- Clean resource release (auto-stops webcam on interruption)

## 🛠 Installation

Run this in your Colab cell to install dependencies:

```python
!pip install ultralytics opencv-python-headless pillow
