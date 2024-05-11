# Paddy Disease Classification: <br>
<br>
- Kaggle Competition Link: [Paddy Doctor](https://www.kaggle.com/competitions/paddy-disease-classification) <br>

## Contents of the repository: <br>
### Notebook-1: Exploring Image models in Pytorch Image Models(Timm):
>  - The notebook uses the dataset given by the competition <br>
>  - It utilizes two robust pretrained models: **a. ResNet26d**, **b. ConvNext_tiny** <br>
>  - The notebook also explores fast.ai library which gives various functionalities such as: `lr_find()` {which suggests an appropriate range of learning rate}, `fine_tune` & `fit_one_cycle()` <br>
---
### Notebook-2: Optimizing the Training Time taken by the used models: <br>
>  - Resizing the input data -> to smaller resolutions. <br>
>  - Adding Preprocessing steps: *a. Squishing*, *b. Cropping*, *c. Padding*, *d. Test time Augmentation*
---
### Notebook-3: Scaling up the models: <br>
>  - This notebook demonstrates the performance of larger image models with larger inputs.<br>
>  - This also demonstrates saving GPU memory by using a technique called `GradientAccumulation`;{as larger models require large amounts GPU memory} <br>
>  - Runs a number of large models: **a. Convnext_in22k_large**, **b. vit_large_patch16_224**, **c. swinv2_large_window12_192_22k**, **d. swin_large_patch4_window7_224** <br>
---
### Notebook-4: Multi-modal Classification: <br>
>  - This notebook demonstrates how to make a multi-target classification using a single model. <br>
>  - The targets to be predicted were selected as: *a. Disease type*, *b. Variety of rice* <br>
>  - A `convnext_in22k_small` model was trained to predict these selected targets, and was finetuned for `epochs=12` & `Learning_rate=0.01`
---
