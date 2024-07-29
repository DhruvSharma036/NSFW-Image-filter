Here's the updated README without the entire source code:

---

# NSFW Image Filter Using ResNet50

This project uses a pre-trained ResNet50 model to create an NSFW (Not Safe For Work) image filter. The filter classifies images into categories such as adult content and violence by leveraging transfer learning. Users can access the dataset, train the model, and make predictions on new images.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Training](#training)
- [Prediction](#prediction)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project uses transfer learning with ResNet50 to build a classifier that can identify inappropriate content in images, specifically focusing on categories such as adult content and violence.

## Dataset

The dataset is organized in the following structure:
```
NSFW image filter/
    └── resnet50_inappropriate_content_detect-master/
        ├── test_images_adult/
        │   ├── normal/
        │   └── porn/
        └── test_images_violence/
            ├── normal/
            └── violence/
```

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/DhruvSharm036/nsfw_image_filter.git
    ```

2. Navigate to the project directory:
    ```sh
    cd nsfw_image_filter
    ```

3. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

Mount Google Drive and verify dataset paths. Use `ImageDataGenerator` for data augmentation and flow images from directories.

## Training

Define the ResNet50 model, add custom layers, and compile it. Train the model using combined generators for both adult content and violence categories.

## Prediction

Load the trained model and use it to make predictions on new images by preprocessing the input and obtaining model predictions.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes or improvements.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
