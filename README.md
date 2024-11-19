# Vehicle Detection and Counting Using YOLOv8 with PyTorch Transfer Learning

## Introduction
The rapid growth of private vehicle usage has made a couple of bad impacts such as traffic management issue and air pollution issue. Vehicle model detection and counting can address these challenges by providing data-driven insights for traffic optimization. Not only that, but also can address like advertising strategies and urban planning. This essay discusses about the development of a vehicle detection model utilizing YOLOv8 and PyTorch Transfer Learning. 

## Methodology

### Data Collection and Preprocessing
- **Dataset**: A custom dataset of 1,667 images was collected by recording videos of urban traffic using a smartphone (Samsung A73).
- **Preprocessing**: The Roboflow platform was used for labeling and augmenting data, ensuring robust model performance under diverse conditions such as varying angles and lighting.

### Model and Training
- **Model**: The YOLOv8 pre-trained model was adapted for car detection.
- **Modifications**: Fine-tuning was performed to specialize the model in detecting and counting cars.
- **Training**:
  - Framework: PyTorch
  - Epochs: 20
  - Input Size: 640x640 pixels
  - Transfer Learning: Enabled leveraging knowledge from the base YOLOv8 model.

### Implementation
- **Detection Mechanism**: The model processes video frames in real-time, identifying vehicles using bounding boxes.
- **Counting Mechanism**: A Centroid Tracker algorithm assigns unique IDs to detected vehicles, ensuring accurate counting across video frames.
- **Challenges Addressed**:
  - Variability in angles and lighting was mitigated by data augmentation and robust model training.

## Results
- **Accuracy**: The model achieved a detection accuracy of **97.92%** during testing.
- **Performance in Real-Time**: Successfully tracked and counted vehicles with unique IDs in live video feeds.
- **Error Analysis**: Minor false positives and misdetections were observed under extreme lighting variations, highlighting areas for further optimization.

## Applications
1. **Traffic Management**:
   - Real-time data can optimize traffic light durations and reduce congestion.
2. **Urban Planning**:
   - Vehicle counts provide insights for infrastructure development.
3. **Advertising**:
   - Accurate traffic density data aids in selecting optimal locations for billboards and campaigns.

## Conclusion
This project demonstrates the potential of integrating YOLOv8 and transfer learning with Centroid Tracking to address traffic challenges. Future work could include expanding the model to detect other vehicle types and improving robustness under extreme environmental conditions.

---

For more details, feel free to check out the [YOLO documentation](https://pjreddie.com/darknet/yolo/) or [my GitHub](https://github.com/ahsanfirdaus1/vehicle-detection-essay) repository.

"I am a panda" 
