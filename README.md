# Capstone-project-Team-1

![image](https://github.com/smaliyu/capstone-project/assets/98468845/6f1bf644-8334-4926-8715-2fcf1da61e8e)

# Brain Tumor Classification Project

This project focuses on the classification of brain tumor images using deep learning techniques leveraging Pytorch framework. The dataset used for this study is the Brain Tumor MRI dataset, which comprises four classes: Glioma, Meningioma, No tumor, and Pituitary. The primary objective is to classify images into one of these classes.

## Dataset Overview

- Total dataset size: 7,023 images
- Training set: 5,712 images
- Testing set: 1,311 images

## Data Preparation

The dataset was obtained from Kaggle and downloaded using the Kaggle API. It was then extracted and processed in Google Colab. The PyTorch DataLoader module was utilized to transform the dataset into PyTorch format. Initially, a series of transformations were applied to the dataset, including resizing, converting it to a tensor, and normalization. A batch size of 32 was used for training.

## Model Performance

The project involved training three different models for 10 epochs, employing a Crossentropy loss function, Adam optimizer, and a learning rate of 0.001 on a GPU device. The table below summarizes the results:

| Model Name      | Training Loss | Training Accuracy | Testing Loss | Testing Accuracy | Time (seconds) |
|-----------------|---------------|-------------------|--------------|------------------|----------------|
| EfficientNet_B0 | 0.2368        | 0.9167            | 0.2461       | 0.9054           | 309.958        |
| EfficientNet_B2 | 0.2763        | 0.9007            | 0.2685       | 0.8986           | 427.855        |
| MobileNet       | 0.0263        | 0.9923            | 0.1065       | 0.9695           | 358.493        |

## Conclusion

Overall, the project demonstrates the effectiveness of different deep learning models in classifying brain tumor images. Further optimizations and fine-tuning can potentially improve model performance.
