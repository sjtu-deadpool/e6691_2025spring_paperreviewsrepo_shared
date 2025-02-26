# Mask R-CNN Training and Prediction

## Overview &#x20;

This repository contains Jupyter Notebook files for training and predicting with Mask R-CNN. &#x20;

## Files &#x20;

- ``: This notebook is used for performing predictions using a pre-trained Mask R-CNN model. &#x20;
- ``: This notebook is used for training Mask R-CNN using multiple GPUs. &#x20;

## Prediction Instructions &#x20;

If you only want to run predictions, please follow these steps: &#x20;

1. **Download Pre-trained Weights  **

   - Before running `main_predict_E.ipynb`, download the necessary weights from the following link: [Mask R-CNN Pre-trained Weights](https://drive.google.com/drive/folders/1X6NgfCWvLtS1EkioZUmeOsWW1V9yptnR?usp=drive_link)   &#x20;
   - Ensure that the downloaded weights are placed in the correct directory as required by the notebook. &#x20;

2. **Run **`` &#x20;

   - Open the Jupyter Notebook. &#x20;
   - Load the pre-trained weights. &#x20;
   - Perform inference using the Mask R-CNN model. &#x20;

## Training Instructions &#x20;

If you wish to train Mask R-CNN from scratch or fine-tune the model, use `train_multi_GPU.ipynb`  :

1. Set up the training dataset. &#x20;
2. Configure the model parameters. &#x20;
3. Run the notebook on a system with multiple GPUs for efficient training. &#x20;

For any issues or questions, please refer to the documentation inside each notebook. Happy coding! &#x20;

