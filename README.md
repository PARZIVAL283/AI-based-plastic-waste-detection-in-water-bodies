# AI-based Plastic Waste Detection in Water Bodies

A computer vision project focused on identifying and localizing plastic waste in aquatic environments using deep learning. The goal is to support environmental monitoring, cleanup planning, and real-time detection of pollution in rivers, lakes, and coastal waters.

## Overview

Plastic pollution is one of the biggest environmental challenges facing water bodies today. Manual monitoring is often slow, expensive, and inconsistent. This project explores an AI-driven approach to automatically detect plastic waste in imagery captured from water environments using object detection models.

This repository contains a notebook-based workflow for:

- loading and preprocessing image data
- annotating or preparing bounding boxes for plastic waste
- training an object detection model
- evaluating model performance
- running inference on new images or video frames

## Problem Statement

Water bodies are frequently affected by plastic waste, including bottles, packaging, fragments, and debris. Detecting these materials at scale is difficult with manual methods alone. Automated AI-based vision systems can help monitor pollution hotspots and support timely cleanup operations.

## Objectives

- Detect plastic waste objects in aquatic scenes
- Reduce dependence on manual inspection
- Support environmental conservation efforts with AI-assisted analysis
- Provide a reproducible workflow for model training and evaluation

## Project Structure

```text
.
├── Project.ipynb         # Main notebook for data exploration, training, and evaluation
├── README.md             # Project documentation
└── ...                   # Additional scripts, data, or model artifacts may be added later
```

## Tech Stack

- Python
- Jupyter Notebook
- OpenCV
- NumPy
- Pandas
- TensorFlow or PyTorch (depending on the model implementation)
- YOLO / object detection framework (if used in the notebook)
- Matplotlib / Seaborn for visualization

## Workflow

1. Collect image data from water bodies and environmental monitoring sources
2. Prepare and clean the dataset
3. Label plastic waste objects in images
4. Train a deep learning object detection model
5. Validate results using metrics such as precision, recall, and mAP
6. Run inference on new images and analyze detection outputs

## Dataset

The project is designed to work with image datasets containing annotated plastic waste instances in aquatic environments. Typical data sources may include:

- public environmental datasets
- manually collected drone or shoreline images
- camera footage from rivers, lakes, or beaches
- annotated benchmark datasets for pollution detection

If you are using a custom dataset, ensure that annotations follow a standard object detection format such as:

- Pascal VOC
- COCO JSON
- YOLO TXT annotations

## Setup

Clone the repository:

```bash
git clone https://github.com/PARZIVAL283/AI-based-plastic-waste-detection-in-water-bodies.git
cd AI-based-plastic-waste-detection-in-water-bodies
```

Create and activate a virtual environment:

```bash
python -m venv venv
source venv/bin/activate   # On Linux/macOS
# venv\Scripts\activate   # On Windows
```

Install dependencies:

```bash
pip install -r requirements.txt
```

If a requirements file is not present yet, install the common packages manually:

```bash
pip install jupyter opencv-python numpy pandas matplotlib tensorflow torch torchvision
```

## Running the Project

Open the notebook:

```bash
jupyter notebook Project.ipynb
```

Then follow the notebook flow for:

- dataset loading
- preprocessing and augmentation
- model training
- evaluation metrics
- inference and visualization

## Model Training Notes

The exact training approach depends on the implementation used in the notebook. Common choices include:

- YOLO-based detection models for fast inference
- Faster R-CNN for higher accuracy in some settings
- SSD models for compact detection pipelines

A typical training pipeline includes:

- splitting data into train/validation/test sets
- normalizing image inputs
- applying augmentation to handle varying water conditions
- monitoring loss and validation metrics
- tuning hyperparameters for better detection accuracy

## Evaluation

The model can be evaluated using standard object detection metrics, such as:

- precision
- recall
- F1 score
- mean Average Precision (mAP)
- IoU-based detection accuracy

Example evaluation steps include:

- comparing predicted bounding boxes with ground-truth labels
- visualizing false positives and false negatives
- analyzing performance across different water conditions

## Use Cases

This project can support:

- environmental monitoring of rivers and coastlines
- detecting pollution before and after cleanup operations
- supporting citizen science and conservation initiatives
- analyzing large image datasets for waste classification and tracking

## Future Improvements

- improve dataset quality and annotation consistency
- add video-based detection to monitor moving water scenes
- optimize the model for edge deployment on drones or mobile systems
- expand class coverage beyond plastic to include other debris types
- deploy as a web application or REST API for field use

## Contributing

Contributions are welcome. If you want to improve the model, add data processing steps, or expand the project scope, please open an issue or submit a pull request.

## License

This project is licensed by Sourodip Das Gupta. It is used for univercity use purpose.

## Contact

Email: sourodipdasgupta283@gmail.com
linkedIn: www.linkedin.com/in/sourodip-das-gupta-3b97a62a6
