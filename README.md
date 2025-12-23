# Task 10: Traffic Sign Recognition

**Student:** Nihat Gok
**ID:** S212
**Seed:** 20240212

## Presentation
[View Presentation Slides](https://drive.google.com/your-link-here)

## Dataset
- **Name:** GTSRB (German Traffic Sign Recognition)
- **Classes:** 10 (Speed limit (30km/h), Priority road, Yield, Stop, No entry, General caution, Road work, Turn right ahead,Ahead only, Keep right)
- **Training samples:** 10,140
- **Test samples:** 4,920

## Model Architecture
- **Type:** MobileNetV2
- **Convolutional layers:** 53
- **Fully connected layers:** 1
- **Total parameters:** 2,236,682

## Training Comparison

### Version 1
- **Learning rate:** 0.0001
- **Batch size:** 32
- **Optimizer:** Adam
- **Test accuracy:** 90.9%

### Version 2
- **Learning rate:** 0.0001
- **Batch size:** 64
- **Optimizer:** Adam
- **Test accuracy:** 90.2%

### Best Result
- **Best version:** Version 1
- **Final test accuracy:** 90.93%
- **Target accuracy:** 88.0%
- **Status:** ✓ Achieved

## Analysis
- **Best performing class:** Speed limit (30km/h)
- **Worst performing class:** Road work
- **Key observations:** By comparing version 1 and version 2, I learned how changes in learning rate and the number of epochs directly affect model performance and stability. A higher learning rate trained faster but was less stable, while a lower learning rate with more epochs gave more consistent results. This comparison helped me understand how tuning hyperparameters improves accuracy and reduces overfitting.

## Files
- `notebook.ipynb`: Complete implementation with both training runs
- `results/training_comparison.png`: Comparison of Version 1 vs Version 2
- `results/confusion_matrix.png`: Confusion matrix from best model
- `results/predictions.png`: Sample predictions
