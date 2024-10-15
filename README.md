# CAR_PLATE YOLO Format Labels

This repository contains labels for car  plates in YOLO format.  

## Table of Contents
- [Introduction](#introduction)
- [Dataset Structure](#dataset-structure)
- [YOLO Label Format](#yolo-label-format)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project provides annotations for car plates in the YOLO (You Only Look Once) format. The labels are designed for use with YOLO models (e.g., YOLOv3, YOLOv4, YOLOv5) and are formatted to work out of the box with YOLO-based object detection frameworks.

## Dataset Structure

The labeling files are organized as follows:

CAR_PLATE_yolo_format_labels-main/
 │ 
 ├── images/ # Directory for images to be labeled 
 │      ├── example.jpg # Example image 
 │    
 ├── labels/ # Directory for YOLO format labels 
 │      ├── example.txt # Example label corresponding to example.jpg 
 │ 
 └── README.md # Project description and details


Each label file in the `labels/` directory corresponds to an image file in the `images/` directory.

## YOLO Label Format

The label files use the YOLO annotation format, which has the following structure:

<class_id> <x_center> <y_center> <width> <height>

- `<class_id>`: The class ID for the object (for car plates, this is `0`).
- `<x_center>`: The normalized x-coordinate of the bounding box center (relative to the image width).
- `<y_center>`: The normalized y-coordinate of the bounding box center (relative to the image height).
- `<width>`: The normalized width of the bounding box.
- `<height>`: The normalized height of the bounding box.

All values are normalized between 0 and 1, where the dimensions are relative to the image size.

## Usage

1. Place your images in the `images/` directory.
2. Create corresponding YOLO format label files in the `labels/` directory, ensuring that each label file has the same name as the image file (but with a `.txt` extension).

## Contributing

Feel free to contribute by submitting pull requests to improve the labeling quality or add more car plate images.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
