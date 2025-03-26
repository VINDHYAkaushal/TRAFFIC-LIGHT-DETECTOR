# TRAFFIC-LIGHT-DETECTOR
Developed a traffic light detector using a YOLO model, capable of processing both images and videos.
I used the yolov3 model to acheive  <img width="834" alt="Screenshot 2025-03-26 at 17 40 31" src="https://github.com/user-attachments/assets/c3b9893f-3705-4c43-950d-0dfda22023ce" />
# Traffic Light Detection with YOLOv8  

This repository contains three trained YOLOv8 models designed to detect traffic lights and classify their colors. The models are available in different sizes—Nano, Small, and Medium—offering a trade-off between speed and accuracy depending on your hardware and requirements.  

## 📂 Models  

| Model File                   | Description                                  |  
|------------------------------|----------------------------------------------|  
| `best_traffic_nano_yolo.pt`  | YOLOv8 Nano – optimized for speed.          |  
| `best_traffic_small_yolo.pt` | YOLOv8 Small – balance between speed & accuracy. |  
| `best_traffic_med_yolo_v8.pt` | YOLOv8 Medium – higher accuracy, but slower. |  

## ⚡ Model Performance  

The following table shows the execution time of each model when tested on a Mac M1 Max (CPU only):  

| Model Size | Execution Time (ms) | Hardware |  
|------------|---------------------|----------|  
| Nano       | 43.7                | Mac M1 Max (CPU) |  
| Small      | 72.1                | Mac M1 Max (CPU) |  
| Medium     | 130.2               | Mac M1 Max (CPU) |  

## 🚀 Usage  

### Running a Live Test  
To test the model in real time using a webcam, run the `livetest.py` script:  

```bash
python livetest.py --model <path_to_model.pt>
