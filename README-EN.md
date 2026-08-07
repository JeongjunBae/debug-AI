# debug-AI

# Solution Approach

- Object Detection
- Classification
- Multilabel-Classification ✔️

# Dataset and Final Performance

We increased the number of crop types and disease types by adding data to the initially provided dataset, which consisted of 3 crop types (Red Bean, Sesame, Soybean), 8 disease types (Red Bean Powdery Mildew, Red Bean Bacterial Leaf Blight, Red Bean Rhizopus, Sesame Bacterial Leaf Spot, Sesame Powdery Mildew, Soybean Downy Mildew, Soybean Wildfire, Soybean Symptoms), and 1 normal type (Soybean).

AI HUB: Additional data for 19 crop types and 42 disease types

Greenhouse Crop Disease Diagnosis Image Introduction ([https://aihub.or.kr/aidata/30729](https://aihub.or.kr/aidata/30729))

Open-field Crop Disease Diagnosis Image Introduction ([https://aihub.or.kr/aidata/30731](https://aihub.or.kr/aidata/30731))

Orchard Fire Blight Captured Image Introduction ([https://aihub.or.kr/aidata/30732](https://aihub.or.kr/aidata/30732))

For normal sesame data, the following dataset was used:

[https://www.kaggle.com/datasets/ravirajsinh45/crop-and-weed-detection-data-with-bounding-boxes](https://www.kaggle.com/datasets/ravirajsinh45/crop-and-weed-detection-data-with-bounding-boxes)

Normal red bean data was provided after requesting Red Bean Leaf data from the authors of the following paper:

[Leaf image-based classification of some common bean cultivars using discriminative convolutional neural networks](https://www.sciencedirect.com/science/article/abs/pii/S0168169920331409)

Here is the fully translated table from the image you provided.

### Crop Disease Dataset & Performance Breakdown

| Crop Name                       | Disease Name                       | Train Images | Eval Images | f1-score             |
| ------------------------------- | ---------------------------------- | ------------ | ----------- | -------------------- |
| **Red Bean**                    | Normal                             | 1083         | 362         | 1.00                 |
|                                 | Powdery Mildew                     | 2268         | 757         | 1.00                 |
|                                 | Bacterial Leaf Blight              | 415          | 139         | 1.00                 |
|                                 | Rhizopus                           | 932          | 311         | 1.00                 |
| **Sesame**                      | Normal                             | 425          | 142         | 1.00                 |
|                                 | Bacterial Leaf Spot                | 2085         | 695         | 0.96                 |
|                                 | Powdery Mildew                     | 113          | 38          | 0.79                 |
| **Soybean**                     | Normal                             | 848          | 283         | 0.97                 |
|                                 | Downy Mildew                       | 1258         | 420         | 0.99                 |
|                                 | Wildfire                           | 817          | 273         | 0.97                 |
|                                 | Bacterial Blight                   | 986          | 329         | 0.96                 |
|                                 | Symptoms                           | 1239         | 413         | 0.99                 |
|                                 | Leaf Spot                          | 375          | 125         | 0.99                 |
| **Eggplant**                    | Normal                             | 375          | 125         | 1.00                 |
|                                 | Leaf Mold                          | 375          | 125         | 1.00                 |
|                                 | Powdery Mildew                     | 243          | 82          | 1.00                 |
| **Pepper**                      | Normal                             | 375          | 125         | 1.00                 |
|                                 | Mild Mottle Virus                  | 375          | 125         | 1.00                 |
|                                 | Leaf Spot                          | 375          | 125         | 1.00                 |
|                                 | Powdery Mildew                     | 375          | 125         | 1.00                 |
| **Sweet Pumpkin**               | Normal                             | 375          | 125         | 1.00                 |
|                                 | Leaf Spot                          | 375          | 125         | 1.00                 |
|                                 | Powdery Mildew                     | 375          | 125         | 1.00                 |
| **Strawberry**                  | Normal                             | 375          | 125         | 1.00                 |
|                                 | Powdery Mildew                     | 375          | 125         | 1.00                 |
| **Lettuce**                     | Normal                             | 375          | 125         | 1.00                 |
|                                 | Sclerotinia Rot                    | 375          | 125         | 1.00                 |
|                                 | Downy Mildew                       | 375          | 125         | 1.00                 |
| **Watermelon**                  | Normal                             | 375          | 125         | 1.00                 |
|                                 | Anthracnose                        | 375          | 125         | 1.00                 |
|                                 | Powdery Mildew                     | 375          | 125         | 1.00                 |
| **Aehobak** _(Korean Zucchini)_ | Normal                             | 375          | 125         | 1.00                 |
|                                 | Leaf Spot                          | 187          | 63          | 0.98                 |
|                                 | Downy Mildew                       | 375          | 125         | 1.00                 |
|                                 | Powdery Mildew                     | 375          | 125         | 0.98                 |
| **Cucumber**                    | Normal                             | 375          | 125         | 1.00                 |
|                                 | Green Mottle Mosaic Virus          | 375          | 125         | 1.00                 |
|                                 | Downy Mildew                       | 332          | 111         | 0.90                 |
|                                 | Powdery Mildew                     | 332          | 111         | 0.89                 |
| **Zucchini**                    | Normal                             | 375          | 125         | 1.00                 |
|                                 | Cucumber Green Mottle Mosaic Virus | 375          | 125         | 1.00                 |
| **Oriental Melon**              | Normal                             | 375          | 125         | 1.00                 |
|                                 | Downy Mildew                       | 351          | 117         | 0.98                 |
|                                 | Powdery Mildew                     | 366          | 123         | 0.98                 |
| **Tomato**                      | Normal                             | 375          | 125         | 1.00                 |
|                                 | Leaf Mold                          | 375          | 125         | 1.00                 |
|                                 | Yellow Leaf Curl Virus             | 375          | 125         | 1.00                 |
|                                 | Leaf Blight                        | 185          | 62          | 1.00                 |
| **Grape**                       | Normal                             | 375          | 125         | 1.00                 |
|                                 | Downy Mildew                       | 183          | 62          | 1.00                 |
| **Radish**                      | Normal                             | 375          | 125         | 1.00                 |
|                                 | Black Spot                         | 375          | 125         | 1.00                 |
|                                 | Downy Mildew                       | 188          | 63          | 0.99                 |
| **Napa Cabbage**                | Normal                             | 375          | 125         | 1.00                 |
|                                 | Black Rot                          | 375          | 125         | 1.00                 |
|                                 | Downy Mildew                       | 371          | 124         | 1.00                 |
| **Cabbage**                     | Normal                             | 375          | 125         | 1.00                 |
|                                 | Sclerotinia Rot                    | 296          | 99          | 0.91                 |
|                                 | Soft Rot                           | 136          | 46          | 0.80                 |
| **Green Onion**                 | Normal                             | 375          | 125         | 1.00                 |
|                                 | Black Spot                         | 375          | 125         | 1.00                 |
|                                 | Downy Mildew                       | 210          | 71          | 0.54                 |
|                                 | Rust                               | 375          | 125         | 0.76                 |
| **Pumpkin**                     | Normal                             | 375          | 125         | 1.00                 |
|                                 | Downy Mildew                       | 174          | 58          | 0.63                 |
|                                 | Powdery Mildew                     | 193          | 65          | 0.71                 |
| **Pear**                        | Normal                             | 375          | 125         | 1.00                 |
|                                 | Fire Blight                        | 375          | 125         | 1.00                 |
| **Apple**                       | Normal                             | 375          | 125         | 1.00                 |
|                                 | Brown Spot                         | 375          | 125         | 0.97                 |
|                                 | Fire Blight                        | 375          | 125         | 0.97                 |
|                                 | Alternaria Leaf Spot               | 375          | 125         | 0.97                 |
| ---                             | ---                                | ---          | ---         | ---                  |
| **Total: 22 Crops**             | **72 Classes (Diseases=50)**       | **33091**    | **11044**   | **Macro Avg: 0.971** |

# [Technique 1] PlantGAN

One difficulty in the plant disease detection problem is that the acquisition difficulty between normal plant images and diseased plant images is different.
Diseased plant images are expensive to acquire because they must be cultivated in isolated environments under expert supervision through virus injections.

By utilizing CycleGAN, you can generate diseased plant images from normal plant images, which are cheaper to acquire.

PlantGAN, which references the LeafGAN paper, is a variant of CycleGAN, identically to LeafGAN.
While LeafGAN uses Grad-CAM for leaf segmentation, PlantGAN utilizes U^2 Net for leaf segmentation.

By applying attention to the leaf through leaf segmentation, CycleGAN can modify only the leaf without generating or altering the background.

# [Technique 2] Crop-aware

One unique aspect of the plant disease detection problem is that identifying the crop type is very easy.
Crop-aware is a method that provides both the image and the crop type together during training and inference.

During training, the backpropagation for other crop types is set to 0, ensuring they are not learned.
During inference, the confidence for other crop types is set to 0, so they are not considered.

# [Technique 3] Augmentation

# Ablation Study

| ![image](https://user-images.githubusercontent.com/80030558/172643212-0fad9854-b2ef-4a3b-9a95-b49902acce0d.png) | ![image](https://user-images.githubusercontent.com/80030558/172643419-f96f3f75-ea4a-45af-ae0a-959b980d0ebd.png) |
| --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |

![image](https://user-images.githubusercontent.com/80030558/172643944-a4bd80e6-ed84-451c-804c-41111a0cc775.png)

# Citation

- Survey

    
[Deep learning models for plant disease detection and diagnosis](https://www.sciencedirect.com/science/article/abs/pii/S0168169917311742)

- GAN

    
[LeafGAN: An Effective Data Augmentation Method for Practical Plant Disease Diagnosis](https://arxiv.org/pdf/2002.10100.pdf)

- Class Imbalance

    
[Emotion Classification with Data Augmentation Using Generative Adversarial Networks](https://arxiv.org/pdf/1711.00648.pdf)
