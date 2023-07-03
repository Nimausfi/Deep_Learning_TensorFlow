
# **Convolutional Neural Network (CNN) with Tensorflow**


### **Summary**
Summary about the entire project (detaset + preprocessing + transfer learning and fine-tuning + models + feature extraction + callbacks (OPTIONAL) + test and evaluate).


### **Dataset**
Dataset can be accessed and downloaded from Kaggle: [Fruits and Vegetables Image Recognition Dataset](https://www.kaggle.com/datasets/kritikseth/fruit-and-vegetable-image-recognition)

This dataset contains images of Fruits and Vegetables:

**Fruits:** banana, apple, pear, grapes, orange, kiwi, watermelon, pomegranate, pineapple, mango.

**Vegetables:** cucumber, carrot, capsicum, onion, potato, lemon, tomato, raddish, beetroot, cabbage, lettuce, spinach, soy bean, cauliflower, bell pepper, chilli pepper, turnip, corn, sweetcorn, sweet potato, paprika, jalepeño, ginger, garlic, peas, eggplant.

++ Create a folder and move images to it (dataset-cover.jpg)


### **Models**

**Transfer Learning:** All pre-trained models were implemented from [TensorFlow Hub](https://www.tensorflow.org/hub) as a starting point, moreover, fine-tuning employed to further training the pre-trained models by updating its weights.

**Fine-Tuning:** To fine-tune the base models, first set its trainable attribute to "True" (unfreezing all of the frozen). Then, since there is a relatively small training dataset, re-freeze every layer except for the last 5 (making them trainable).

++ Add name of models and link to their source codes

| Model            |                                      Links                          |
| ----------------- | ------------------------------------------------------------------ |
| EfficientNetB0_Model | ![#00d1a0](https://via.placeholder.com/10/00b48a?text=+) #00d1a0 |
| EfficientNetB4_Model | ![#00d1a0](https://via.placeholder.com/10/00b48a?text=+) #00d1a0 |
| EfficientNetV2B0_Model | ![#00d1a0](https://via.placeholder.com/10/00b48a?text=+) #00d1a0 |
| ResNet50_Model | ![#00d1a0](https://via.placeholder.com/10/00b48a?text=+) #00d1a0 |
| ResNet101_Model | ![#00d1a0](https://via.placeholder.com/10/00b48a?text=+) #00d1a0 |
| ResNet101V2_Model | ![#00d1a0](https://via.placeholder.com/10/00b48a?text=+) #00d1a0 |


[<kbd> <br> KeyBinding Button <br> </kbd>][KBD]

[![Button Shield]][Shield]

[Button Shield]: https://img.shields.io/badge/Shield_Buttons-37a779?style=for-the-badge

### **Performance Evaluation**

Learning curves => Training and Validation Loss


### **Links**



