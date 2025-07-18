# NIR Vein Segmentation

This project focuses on the segmentation of veins from Near-Infrared (NIR) images using deep learning. The primary goal is to accurately identify and delineate vein patterns, which has applications in medical imaging and biometrics. This repository provides the necessary code to train and test a vein segmentation model.

***

## 🌟 Features

* **Vein Segmentation:** Utilizes a U-Net-based architecture for semantic segmentation of veins in NIR images.
* **Data Augmentation:** Includes scripts for data augmentation to improve model robustness and accuracy.
* **Pre-trained Models:** Provides pre-trained models for immediate inference and testing.
* **Graphical User Interface (GUI):** An optional GUI is available for easy on-device deployment and visualization of segmentation results.
* **Dataset:** Comes with a dataset of NIR forearm images and their corresponding annotated masks.

***

## 🖼️ Dataset

The dataset contains NIR images of forearms and their corresponding ground truth masks. The data is organized into training and validation sets.

* **Images:** Raw NIR images of forearms.
* **Masks:** Binary masks where the vein pixels are labeled.

The dataset is available in the `/dataset` directory.

***

## ⚙️ Installation

To get started with this project, clone the repository and install the required dependencies.

```bash
git clone [https://github.com/your-username/nir-vein_segmentation.git](https://github.com/your-username/nir-vein_segmentation.git)
cd nir-vein_segmentation
pip install -r requirements.txt
```
🚀 Usage

You can either train the model from scratch or use the pre-trained models for inference.

***
### Training

To train the model, run the `train.py` script:

```bash
python train.py

```
Make sure to specify the path to your dataset in the script if it's not in the default location.


Inference
For inference on new images, use the inference.py script:

```bash
python inference.py --image_path /path/to/your/image.png
```
The segmented output will be saved in the /output directory.

GUI
To use the graphical user interface for real-time segmentation with a connected NIR camera:

```bash
python gui.py
```

🏗️ Model Architecture
The core of this project is a U-Net based model, a convolutional neural network architecture that is well-suited for biomedical image segmentation tasks. The U-Net architecture consists of an encoder and a decoder path, with skip connections that allow for precise localization.

***

📜 License
This project is licensed under the MIT License. See the LICENSE file for details.








