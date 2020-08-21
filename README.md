# Food-101-Challenge
## Summary
This repo contains notebooks training a classification model on the Food-101 dataset.
Food-101  is a dataset consisting of 101 classes with 1000 images per class. For each class, 250 images are reserved as for the test set. The dataset is difficult for a number of reasons. There's a small amount of training data for each class. Many classes look similar to each other (ex steak vs filet mignon). Many images in the dataset have poor lighting or framing. Several images contain multiple correct classes (ex burgers + fries), despite the dataset being structured as a single class classification problem. On top of all that there are a number of mislabeled images.

## Notebooks
- **food101-eda** Exploratory Data Analysis on the dataset, in order to get familiar with the dataset, the images. Also in this notebook I displayed visualization of data augmentation, a visual experience of how image augmentation can increase data diversity and thus help the model training.
- **food-101-resnet-256** shows the ResNet50 model trained on 256X256 images, with 18 total epochs, Top-1 accuracy only got to 81.4%
- **food-101-resnet-512** shows the ResNet50 model trained on 512X512 images, with only 10 epochs, Top-1 accuracy only got to 81.5%
- **food-101-resnet-224-512** shows the ResNet50 model sequentially trained on 224X224 and 512X512 images, top-1 accuracy achieved 89.63% and top-5 accuracy achieved 98.04%
