
---

# Odometer Number Detection and Extraction

This project implements a two-step process to detect and extract odometer numbers from images using YOLOv8 Nano for object detection and EasyOCR for text recognition. 
## Project Overview

This solution was designed to automate the insurance process.
. It utilizes YOLOv8 Nano for its efficiency in environments with limited computational resources, and EasyOCR for its high accuracy in general OCR tasks.

Annotated Odometer Dataset: [Car Odometers](https://drive.google.com/drive/folders/1GH88J6Jf7KsAvqnwlPEjvGVHpedEmWFA?usp=sharing) 

## Key Features

- **Object Detection**: Uses YOLOv8 Nano to locate the odometer in an image.
- **Text Recognition**: Applies EasyOCR to extract numbers from the detected odometer region.
- **Optimized for Limited Resources**: Suitable for platforms with restricted computational capabilities like Google Colab.
- **Simple Setup**: Minimal configuration is needed to get the project up and running.


## How It Works

- **Object Detection with YOLOv8 Nano**: The model identifies the region containing the odometer based on the learned features from the training dataset.
- **Text Recognition with EasyOCR**: Numeric information is extracted from the identified ROI using OCR technology.

## Smart Odometer Reader Results
![image](https://github.com/PouriaAzadehR/Smart-Odometer-Reader/assets/93463377/f21706c5-344f-4a29-94fd-4704fbd2f221)
![image](https://github.com/PouriaAzadehR/Smart-Odometer-Reader/assets/93463377/0704c2fa-e245-4afc-864b-691643b855c2)
![image](https://github.com/PouriaAzadehR/Smart-Odometer-Reader/assets/93463377/cfea80b3-b7f4-4190-92bf-23ccae2894dc)

## YOLO Results
![image](https://github.com/PouriaAzadehR/Smart-Odometer-Reader/assets/93463377/6ef79637-cdda-4ef3-8dc7-c8b9850ab70a)
![image](https://github.com/PouriaAzadehR/Smart-Odometer-Reader/assets/93463377/32449d57-178d-41d7-ac2c-8c5363899e28)
![image](https://github.com/PouriaAzadehR/Smart-Odometer-Reader/assets/93463377/14576d8a-5fab-4195-89d8-2c6de584adf8)




## Contributing

Contributions to this project are welcome! Please fork the repository and submit a pull request with your features or fixes.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Thanks to the MakeSense.ai team for their intuitive labeling tool.
- The YOLO and EasyOCR communities for their outstanding open-source contributions.

---

