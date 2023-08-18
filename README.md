# **Deep Convolutional Neural Networks for Image Classification using Transfer Learning**

## **Dataset**
Dataset can be accessed and downloaded from Kaggle platform: [Fruits and Vegetables Image Recognition Dataset](https://www.kaggle.com/datasets/kritikseth/fruit-and-vegetable-image-recognition)

This dataset contains images of fruits and vegetables, and divided into three folders: train (100 images each), test (10 images each), and validation (10 images each).

**Fruits:** banana, apple, pear, grapes, orange, kiwi, watermelon, pomegranate, pineapple, mango.

**Vegetables:** cucumber, carrot, capsicum, onion, potato, lemon, tomato, raddish, beetroot, cabbage, lettuce, spinach, soy bean, cauliflower, bell pepper, chilli pepper, turnip, corn, sweetcorn, sweet potato, paprika, jalepeño, ginger, garlic, peas, eggplant.

<p align="center"> 
<img src="readme_images/dataset_cover.jpg" width=1100>

## **Models**

Transfer learning is a technique in machine learning where a model developed for a task is utilized as the initial point for a model on another task. This method is particularly favored in deep learning where pre-trained models are leveraged to tackle computer vision and natural language processing tasks considering the extensive compute and time resources required to create neural network models for such problems. Transfer learning offers efficient and effective solutions by utilizing the significant performance gains achieved in similar domains.

**Transfer Learning:** All pre-trained models were implemented from [TensorFlow Hub](https://www.tensorflow.org/hub) as a starting point, moreover, fine-tuning was employed to further training the models by updating their weights.

**Fine-Tuning:** To fine-tune the base models, first set its trainable attribute to "True" (unfreezing all of the frozen). Then, since there is a relatively small training dataset, re-freeze every layer except for the last 5 (making them trainable). Check the following link to learn more about the [trainable attributes.](https://keras.io/guides/transfer_learning/)

<br />

| **EfficientNet Models**   | **ResNet Models**     |
| :--:                  | :--:              |
| [EfficientNetB0](https://github.com/Nimausfi/CNN_TensorFlow/blob/main/EfficientNetB0_Model.ipynb)        | [ResNet50](https://github.com/Nimausfi/CNN_TensorFlow/blob/main/ResNet50_Model.ipynb)          |
| [EfficientNetB4](https://github.com/Nimausfi/CNN_TensorFlow/blob/main/EfficientNetB4_Model.ipynb)        | [ResNet101](https://github.com/Nimausfi/CNN_TensorFlow/blob/main/ResNet101_Model.ipynb)         |
| [EfficientNetV2B0](https://github.com/Nimausfi/CNN_TensorFlow/blob/main/EfficientNetV2B0_Model.ipynb)      | [ResNet101V2](https://github.com/Nimausfi/CNN_TensorFlow/blob/main/ResNet101V2_Model.ipynb)       |


## **Performance Evaluation**

Results for evaluating predictions such as confusion matrix, f1 score for each class, and finding most wrong predictions can be found in the source codes.


**Learning curves for training and validation metrics** (fine-tuned EfficientNetB0 model)

<img src="readme_images/learning_curves.jpg" width=400>


**Comparing the accuracy scores of base and fine-tuned models on the whole test dataset**

|  **Models**            |   **Accuracy (base models)**  |  **Accuracy (fine-tuned models)**    |
| :--:                   | :--:                          | :--:                                 |
|  **EfficientNetB0**    |     89.97% 	                 |     **93.31%**                       |
|  **EfficientNetB4**    |     88.57% 	                 |     91.64%                           |
|  **EfficientNetV2B0**  |     89.13% 	                 |     93.03%                           |
|  **ResNet50**          |     **91.92%**                |     90.52%                           |
|  **ResNet101**         |     89.69% 	                 |     92.20%                           |
|  **ResNet101V2**       |     90.52%     		 |     91.08%  	                        |


**Visualizing predictions on custom images**

<img src="readme_images/custom_imgs.jpg" width=600>


