Detecting bacterial flagellar motors in electron microscopy images using YOLOv8 object detection.

Why detecting bacterial motors !? 

Manually identifying bacterial flagellar motors in microscopy images is time-consuming and requires expert knowledge. This automated detection system can:
- Speed up the analysis workflow for biologists
- Provide consistent detection across different images
- Help researchers process large datasets efficiently
- Serve as a foundation for more advanced detection systems

 Results

- mAP50: 87.54%
- mAP50-95: 51.97%


The model performs well but has room for improvement for higher IOU thresholds  - perfect for further research and optimization!

What I Used

 Model & Framework
- YOLOv8l (Large variant)
- Ultralytics 8.3.176
- PyTorch 2.6.0+cu124

Hardware
- GPU: NVIDIA Tesla T4 (15GB VRAM) [ Use collab pro for better perfomance using good gpu with more RAM]
- Platform: Google Colab

 Training Configuration
- Epochs: 200
- Image Size: 940px
- Batch Size: 6
- Patience: 10 (early stopping)

Data Augmentation
- Rotation (±10°)
- Translation (10%)
- Scaling (20%)
- Horizontal Flip (50%)
- Mosaic Augmentation

 Key Libraries
```
ultralytics
torch
opencv
matplotlib
```

Quick Start

```bash
# Install dependencies
pip install ultralytics

# Train the model
python training_script.py
```

The complete code is available in this repository. Just mount your Google Drive, upload the dataset, and you're good to go!

 Project Structure
```
├── training_script.py          # Main training code
├── runs/detect/                # Training outputs
│   └── motor_detector_v8x_high_accuracy/
│       ├── weights/
│       │   └── best.pt        # Trained model
│       └── results.png        # Training curves
└── yolo_data/                 # Dataset directory
```

---

## Research Collaborations & Contributions ## 

I'm Jayanth  I am actively working on multiple research projects and am open to collaborations in machine learning, computer vision, and biological image analysis!

If you're interested in:
- Improving this bacterial motor detection system
- Exploring novel architectures for microscopy images
- Joint research projects in ML/CV
- Publishing research papers together
- Any other research collaboration

Please feel free to reach out !! 

Email: jayanth9b.vhs@gmail.com
               or 
       jayanthadavi@gmail.com

I'm looking for people who want to collaborate, contribute, and build something meaningful together. Whether you're a researcher, student, or just someone passionate about ML - let's connect and workhard ! 
