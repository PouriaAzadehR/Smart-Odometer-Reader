Odometer number detection and extraction project is for automating insurance process.
---

# Odometer Number Detection and Extraction

This project implements a two-step process to detect and extract odometer numbers from images using YOLOv8 Nano for object detection and EasyOCR for text recognition. 
## Project Overview

This solution was designed to accurately identify and read odometer numbers from various vehicle images. It utilizes YOLOv8 Nano for its efficiency in environments with limited computational resources, and EasyOCR for its high accuracy in general OCR tasks.

## Key Features

- **Object Detection**: Uses YOLOv8 Nano to locate the odometer in an image.
- **Text Recognition**: Applies EasyOCR to extract numbers from the detected odometer region.
- **Optimized for Limited Resources**: Suitable for platforms with restricted computational capabilities like Google Colab.
- **Simple Setup**: Minimal configuration is needed to get the project up and running.

## Prerequisites

- Python 3.x
- OpenCV
- EasyOCR
- PyTorch

Ensure all dependencies are installed using pip:

```bash
pip install opencv-python-headless easyocr torch
```

## Installation

Clone this repository to your local machine:

```bash
git clone https://github.com/your-repository/odometer-recognition.git
cd odometer-recognition
```

## Usage

To use this project, follow these steps:

1. **Prepare your dataset**: Place your images in the `input_images` directory.

2. **Run Detection**: Execute the object detection script to locate odometers:

```bash
python detect_odometers.py
```

3. **Extract Numbers**: Run the OCR script to extract numbers from detected regions:

```bash
python extract_numbers.py
```

Results will be saved in the `output` directory.

## Configuration

Edit the `config.json` file to adjust the input and output paths, and modify the model parameters if necessary:

```json
{
    "input_dir": "input_images",
    "output_dir": "output",
    "yolo_config": {
        "model_size": "640x640",
        "weights_path": "models/yolov8_nano_weights.pth"
    }
}
```

## How It Works

- **Object Detection with YOLOv8 Nano**: The model identifies the region containing the odometer based on the learned features from the training dataset.
- **Text Recognition with EasyOCR**: Numeric information is extracted from the identified ROI using OCR technology.

## Smart Odometer Reader Results
![image](https://github.com/PouriaAzadehR/Smart-Odometer-Reader/assets/93463377/f21706c5-344f-4a29-94fd-4704fbd2f221)
![image](https://github.com/PouriaAzadehR/Smart-Odometer-Reader/assets/93463377/0704c2fa-e245-4afc-864b-691643b855c2)
![image](https://github.com/PouriaAzadehR/Smart-Odometer-Reader/assets/93463377/cfea80b3-b7f4-4190-92bf-23ccae2894dc)

## YOLO Results
![image](https://github.com/PouriaAzadehR/Smart-Odometer-Reader/assets/93463377/6ef79637-cdda-4ef3-8dc7-c8b9850ab70a)
![image](https://github.com/PouriaAzadehR/Smart-Odometer-Reader/assets/93463377/14576d8a-5fab-4195-89d8-2c6de584adf8)
![image](https://github.com/PouriaAzadehR/Smart-Odometer-Reader/assets/93463377/32449d57-178d-41d7-ac2c-8c5363899e28)



## Contributing

Contributions to this project are welcome! Please fork the repository and submit a pull request with your features or fixes.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Thanks to the MakeSense.ai team for their intuitive labeling tool.
- The YOLO and EasyOCR communities for their outstanding open-source contributions.

---

