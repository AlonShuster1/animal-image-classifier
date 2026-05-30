# Animal Image Classifier

A deep learning project for classifying images of 10 different animals. Built as part of a university deep learning course.

## What it does

Takes an image and predicts which of the following animals it contains:
dog, cat, horse, cow, sheep, elephant, butterfly, chicken, spider, squirrel

## Models

**TinyVGG (baseline)** — a custom CNN built from scratch, inspired by the VGG architecture. Three convolutional blocks with batch normalization, dropout, and a weighted sampler to handle class imbalance. Reached ~85% test accuracy after 45 epochs.

**ResNet50 (transfer learning)** — we froze the pretrained backbone and replaced the classifier head with our own. Reached ~98% test accuracy in just 10 epochs.

## Dataset

[Animals-10](https://www.kaggle.com/datasets/alessiocorrado99/animals10) from Kaggle — around 28,000 images split 80/20 train/test.

## Stack

- Python, PyTorch, torchvision
- Google Colab (GPU)
- matplotlib for visualizations

## Results

| Model | Test Accuracy |
|-------|--------------|
| TinyVGG (scratch) | ~85% |
| ResNet50 (fine-tuned) | ~98% |
