# Soccer Player & Ball Tracking with YOLOv and DeepSORT

## 📋 Project Overview

This project performs real-time soccer player and ball tracking using a fine-tuned YOLOv model for detection and DeepSORT for consistent identity tracking. It ensures that each player maintains a single consistent ID across frames, even after reappearing in the scene.

---

## ⚙️ Setup Instructions

### 1. Clone the Repository and Prepare Files

* Place your input video inside the `input/` folder.
* Ensure your YOLOv8 fine-tuned model (e.g., `yolov.pt`) is in the project root directory.

### 2. (Recommended) Create a Virtual Environment

```bash
conda create -n football_re_id python=3.10 -y
conda activate football_re_id
```

### 3. Install Dependencies

Make sure the following packages are installed:

```bash
pip install -r requirements.txt
```

If you don’t have a `requirements.txt`, manually install:

```bash
pip install ultralytics==8.0.20
pip install deep_sort_realtime
pip install opencv-python
pip install numpy==1.26.4
```

---

## ▶️ Running the Tracker

1. Launch Jupyter Notebook:

```bash
jupyter notebook
```

2. Open `yolo11_deepsort_reid.ipynb` and run all cells.

* Input video path should be set to `input/15sec_input_720p.mp4`
* Output video will be saved to `outputs/tracked_output.mp4`
* Model path should be set to your fine-tuned `yolov.pt`

---

## 📦 Dependencies

| Package              | Version    |
| -------------------- | ---------- |
| Python               | 3.10.x     |
| Ultralytics (YOLO)   | 8.0.20     |
| torch                | 2.1.0      |
| torchvision          | compatible |
| numpy                | 1.26.4     |
| OpenCV               | latest     |
| deep\_sort\_realtime | latest     |

---
