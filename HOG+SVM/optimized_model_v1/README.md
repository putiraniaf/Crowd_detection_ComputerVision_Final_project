# Optimized Crowd Detector - v1.0

## Model Information
- **Version**: v1.0
- **Created**: 2025-12-17 18:40:32
- **Type**: HOG + SVM with optimized post-processing

## Files
- `body_detector_svm_optimized.pkl` - Trained SVM classifier
- `feature_scaler_optimized.pkl` - Feature scaler
- `config_optimized.json` - Optimized configuration parameters
- `model_info.json` - Model metadata and usage info

## Quick Start

```python
from improved_detector_loader import load_optimized_detector

# Load model
detector = load_optimized_detector("/content/drive/MyDrive/crowd_body_detection/optimized_model_v1")

# Load image
import cv2
image = cv2.imread("test_image.jpg")

# Detect people
boxes, confidences = detector.detect(image)

# Visualize
result = detector.visualize_detections(image, boxes, confidences)
cv2.imwrite("result.jpg", result)

print(f"Detected {len(boxes)} people")
```

## Parameters
- **min_confidence**: 7.5
- **nms_threshold**: 0.2
- **step_size**: 32
- **max_boxes**: 30

## Performance
- Precision: 70-80%
- Recall: 65-75%
- False Positive Rate: Low to Medium

## Notes
Model ini sudah dioptimalkan untuk mengurangi false positives dan memberikan hasil deteksi yang lebih akurat pada crowd scenes.
