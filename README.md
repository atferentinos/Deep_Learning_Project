# Deep_Learning_Project

# Classifying Ancient Art with Neural Nets
A deep learning project to classify ancient Greek, Roman, and Egyptian artwork by culture, medium, and time period.

## Authors
- Becky Desrosiers (rn7ena@virginia.edu)
- Alexandra Ferentinos (kzk8qq@virginia.edu)
- Peter Landers (bjs6pj@virginia.edu)
- Brendan Jalali (bdj9wf@virginia.edu)

University of Virginia, School of Data Science

## Project Overview
This project implements deep learning techniques to classify ancient artwork across three dimensions:
- Culture (Greek, Roman, Egyptian)
- Medium (Architecture, Painting, Sculpture)
- Time Period (Early, Middle, Late)

The final model achieved approximately 50% accuracy using transfer learning with ResNet50 architecture and SE blocks.

## Model Architecture
The project uses three separate classifier sub-models:
- Culture classifier
- Medium classifier  
- Time period classifier

Each sub-model uses:
- 224x224x3 input layer
- Data augmentation
- ResNet50 with transfer learning
- SE (Squeeze-and-Excitation) blocks
- Global Average Pooling
- Fully connected layers with dropout

## Key Features
- Transfer learning using ResNet50
- SE (Squeeze-and-Excitation) blocks for improved performance
- Data augmentation including random flips, rotations, zooming, brightness and contrast adjustments
- Batch normalization and gradient clipping for training stability
- Adam optimizer with exponential decay learning rate

## Results
Final model performance:
- Culture: 46.63% validation accuracy
- Medium: 45.16% validation accuracy  
- Time: 56.60% validation accuracy
- Overall: 50.66% accuracy

## Project Structure
```bash
/ClassicalArt_Project/
├── wrapper.ipynb          # Main model coordinator
├── culture_model/        # Culture classification submodel
├── medium_model/        # Medium classification submodel 
└── time_model/         # Time period classification submodel
```
