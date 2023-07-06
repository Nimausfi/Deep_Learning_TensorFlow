
# **Deep Learning with TensorFlow**


### **Summary**
Summary about the entire project (detaset + preprocessing + transfer learning and fine-tuning + models + feature extraction + callbacks (OPTIONAL) + test and evaluate).

+ confusion matrix + F-1 scores for each classes

### **Dataset**
Dataset can be accessed and downloaded from Kaggle: [Fruits and Vegetables Image Recognition Dataset](https://www.kaggle.com/datasets/kritikseth/fruit-and-vegetable-image-recognition)

This dataset contains images of fruits and vegetables, and divided into three folders: train (100 images each), test (10 images each), and validation (10 images each).

**Fruits:** banana, apple, pear, grapes, orange, kiwi, watermelon, pomegranate, pineapple, mango.

**Vegetables:** cucumber, carrot, capsicum, onion, potato, lemon, tomato, raddish, beetroot, cabbage, lettuce, spinach, soy bean, cauliflower, bell pepper, chilli pepper, turnip, corn, sweetcorn, sweet potato, paprika, jalepeño, ginger, garlic, peas, eggplant.

++ Create a folder and move images to it (dataset-cover.jpg)

### **Models**

**Transfer Learning:** All pre-trained models were implemented from [TensorFlow Hub](https://www.tensorflow.org/hub) as a starting point, moreover, fine-tuning employed to further training the pre-trained models by updating its weights.

**Fine-Tuning:** To fine-tune the base models, first set its trainable attribute to "True" (unfreezing all of the frozen). Then, since there is a relatively small training dataset, re-freeze every layer except for the last 5 (making them trainable).

<br />
<br />

| EfficientNet Models   | ResNet Models     |
| :--:                  | :--:              |
| [EfficientNetB0](https://github.com/Nimausfi/CNN_TensorFlow/blob/main/EfficientNetB0_Model.ipynb)        | [ResNet50](https://github.com/Nimausfi/CNN_TensorFlow/blob/main/ResNet50_Model.ipynb)          |
| [EfficientNetB4](https://github.com/Nimausfi/CNN_TensorFlow/blob/main/EfficientNetB4_Model.ipynb)        | [ResNet101](https://github.com/Nimausfi/CNN_TensorFlow/blob/main/ResNet101_Model.ipynb)         |
| [EfficientNetV2B0](https://github.com/Nimausfi/CNN_TensorFlow/blob/main/EfficientNetV2B0_Model.ipynb)      | [ResNet101V2](https://github.com/Nimausfi/CNN_TensorFlow/blob/main/ResNet101V2_Model.ipynb)       |


<br />
<br />


### **Performance Evaluation**

Learning curves for training and validation metrics (fine-tuned EfficientNetB0 model)

++ Add learning_curves.jpg

Comparing the accuarcy scores of base and fine-tuned models on the whole test dataset

++ Create a table to compare the accuarcy results

Visualizing predictions on custom images

++ Add custom_imgs
