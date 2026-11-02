
# Deep Learning PR 3 – Computer Vision

**Topics:** Morphological Operations, Bitwise Operations, Image Histograms, YuNet Face Detection, YOLO Object Detection

## 1. Project Overview

This project demonstrates a computer vision workflow that starts with classical image-processing techniques and progresses to deep-learning-based detection. It uses OpenCV for image processing and YuNet face detection, and Ultralytics YOLOv8n for object detection.

## 2. Project Objectives

- Apply erosion, dilation, opening and closing to binary images.
- Demonstrate bitwise AND, OR, XOR and NOT operations.
- Generate grayscale and BGR colour histograms.
- Study brightness and contrast adjustment using alpha and beta.
- Detect faces using the pretrained YuNet model.
- Detect everyday objects using pretrained YOLOv8n.
- Combine face and object detection in an integrated video pipeline.
- Compare processing speed using frames per second (FPS).

## 3. Project Structure

```text
PR3_Computer_Vision/
├── CV_PR3.ipynb
├── CV_PR3.html
├── README.md
├── requirements.txt
├── plots/
│   ├── morphology_grid.png
│   ├── bitwise_operations.png
│   ├── histogram_comparison.png
│   ├── face_detection_comparison.png
│   ├── yolo_detections.png
│   └── fps_comparison.png
├── results/
│   ├── task3_results/
│   ├── task4_results/
│   └── task5_results/
└── video/
    └── CV_PR3_YourName_GRID.mp4
```

Add your actual notebook, exported HTML, generated plots, results and video to the folders. Do not leave placeholder files in the final submission.

## 4. Tools and Technologies

- Python 3
- OpenCV
- NumPy
- Matplotlib
- Ultralytics YOLOv8
- Google Colab / Jupyter Notebook
- YuNet pretrained ONNX face detector
- YOLOv8n pretrained on the COCO dataset

## 5. Project Tasks

### Task 1 – Environment Setup, Image I/O & Morphological Operations

Loaded and inspected images, converted images to grayscale and binary format, and applied erosion, dilation, opening and closing. Compared rectangular, elliptical and cross-shaped structuring elements at different kernel sizes.

### Task 2 – Bitwise Operations & Image Histograms

Created binary masks and applied AND, OR, XOR and NOT operations. Demonstrated masked image regions and overlay use cases. Generated grayscale and BGR channel histograms and studied brightness and contrast adjustments using `cv2.convertScaleAbs()`.

### Task 3 – Face Detection with YuNet

Loaded the pretrained YuNet ONNX face detector and applied it to static images and video frames. Displayed face bounding boxes, five facial landmarks and confidence scores. Tested score thresholds and demonstrated face-region blurring for privacy.

### Task 4 – Object Detection with YOLOv8

Loaded the pretrained YOLOv8 Nano model (`yolov8n.pt`) and detected objects in images and video. Displayed bounding boxes, class labels and confidence scores. Experimented with confidence and IoU thresholds and summarized detections by class.

### Task 5 – Integrated Pipeline & Final Comparison

Combined YuNet face detection and YOLO object detection on video frames. Measured FPS for face detection, object detection and the combined pipeline. Prepared a final comparison of the techniques used in Tasks 1–4.

## 6. Dataset and Model Sources

- OpenCV sample images: https://github.com/opencv/opencv/tree/master/samples/data
- OpenCV Zoo (YuNet model): https://github.com/opencv/opencv_zoo
- Ultralytics YOLOv8 documentation: https://docs.ultralytics.com/
- YOLOv8n weights: automatically downloaded by `YOLO("yolov8n.pt")` on first use.

Use your own images and video where appropriate. Ensure you have permission to use and share any personal images or video included in the public repository.

## 7. Installation and Setup

Install the required packages:

```bash
pip install -r requirements.txt
```

Open `CV_PR3.ipynb` in Google Colab or Jupyter Notebook and run the cells in order. The YuNet ONNX model must be available at the path used in the notebook. YOLOv8n weights are downloaded automatically on first use.

## 8. Results and Plots

Place the actual output plots in the `plots/` directory and add a short caption for each:

| Plot | Description |
|---|---|
| `morphology_grid.png` | Original/binary image and morphological operation results |
| `bitwise_operations.png` | Input masks and bitwise operation outputs |
| `histogram_comparison.png` | Grayscale/colour histograms and brightness/contrast comparison |
| `face_detection_comparison.png` | YuNet face detections, landmarks and confidence scores |
| `yolo_detections.png` | YOLO object detections with labels and confidence scores |
| `fps_comparison.png` | FPS comparison of YuNet, YOLO and the combined pipeline |

Only list plots that you have actually generated and checked.

## 9. Final Performance Summary

Enter the actual values measured by your notebook. Do not estimate or invent FPS values.

| Pipeline | Average FPS |
|---|---:|
| YuNet face detection | Add measured value |
| YOLO object detection | Add measured value |
| Combined pipeline | Add measured value |

## 10. Video Demonstration

**Project video:** [Paste your Google Drive / YouTube / other accessible video link here]

The demonstration should be 5–10 minutes and show your face and screen. Explain the four main concepts and demonstrate the face-detection, YOLO and integrated pipeline outputs.

## 11. Conclusion

This project explores classical image processing and deep-learning-based computer vision. Morphological and bitwise operations provide useful image-processing tools, while YuNet and YOLOv8 provide face and general object detection. The integrated pipeline demonstrates how different computer vision techniques can be combined and how their processing speed can be compared.

## 12. Author

**Name:** Swarna Pathak  
Project demonstration video :(https://drive.google.com/file/d/1PpKO3dyhZoJutfyvHRMqbybIZbLFmtoT/view?usp=sharing)
