# **Instance and Semantic Segmentation**

## U-Net and DeepLabv3

Omri Habot (oh2263)

Junyu Hu (jh4930) 

Jinsong Liu (jl6850) 

### U-Net Cars Segmentation

#### Dataset
 The dataset used for this project is contained in `car_data.zip`. Due to its large size, please download it from the following link: 

🔗 [Download car_data.zip](https://drive.google.com/file/d/11_LVaBJaPL9To7xIP3yuijC22Hib56Q-/view?usp=sharing) 

📌 **Note:** You must use a **LionMail (Columbia University)** email account to access the file. After downloading, extract `car_data.zip` before running the notebook.

### DeepLabv3 Model Demo - Semantic Segmentation with PyTorch

The Jupyter Notebook provides a hands-on demonstration of using *DeepLabv3, a state-of-the-art deep learning model for **semantic segmentation*. The notebook guides you through the following steps:

- *Downloading DeepLabv3: Load the model from **Torch Hub* with different backbone architectures (e.g., ResNet-101, MobileNetV3).
- *Preparing an Image for Inference*: Process an input image to match the model's expected format.
- *Running Inference*: Use DeepLabv3 to generate segmentation masks.
- *Visualizing Results*: Overlay the predicted segmentation mask onto the original image for clear interpretation.

This demo is ideal for exploring DeepLabv3’s capabilities and understanding how to apply it to real-world image segmentation tasks.
