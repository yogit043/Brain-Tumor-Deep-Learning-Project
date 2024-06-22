# Brain Tumor Detection using CNN

## 📓 Notebook Overview

The `Brain_tumor.ipynb` notebook contains the following key sections:

### Data Loading and Preprocessing:
- Loads MRI scan images from the dataset.
- Performs preprocessing steps including:
  - Image resizing and normalization
  - Conversion to grayscale
  - Gaussian blur application
  - Thresholding
  - Erosion and dilation
  - Contour finding for brain extraction

### Exploratory Data Analysis (EDA):
- Visualizes the distribution of brain tumor images.
- Displays sample images from each class.
- Analyzes class imbalance in the dataset.

### Data Augmentation:
- Implements data augmentation techniques to balance the dataset and increase model robustness.
- Augmentation includes rotation, width/height shifts, shear, horizontal flip, and brightness adjustments.

### Model Building:
- Utilizes transfer learning with VGG19 as the base model.
- Defines a custom architecture on top of VGG19 for tumor detection.
- Implements three model versions:
  1. Frozen CNN (VGG19 layers frozen)
  2. Partially unfrozen CNN (last few layers of VGG19 unfrozen)
  3. Fully unfrozen CNN

### Model Training:
- Trains the CNN models on the augmented dataset.
- Implements callbacks for early stopping, model checkpointing, and learning rate reduction.
- Uses Stochastic Gradient Descent (SGD) optimizer with momentum.

### Evaluation and Results:
- Evaluates each model's performance on validation and test sets.
- Displays accuracy, loss, and other relevant metrics.
- Visualizes training and validation accuracy/loss curves.

## 🏆 Results

Our models achieved the following accuracies:
1. Frozen CNN: [Insert accuracy here]
2. Partially unfrozen CNN: [Insert accuracy here]
3. Fully unfrozen CNN: [Insert accuracy here]

Detailed performance metrics and visualizations are available in the notebook.

## 🔮 Future Development

In future iterations of this project, we plan to:

1. **Expand Dataset**: Incorporate more diverse and larger datasets to improve model robustness and generalizability.
2. **Model Optimization**: Experiment with different architectures and hyperparameters to enhance model performance.
3. **Real-time Detection**: Develop a real-time detection system that can be integrated into medical imaging devices.
4. **Explainability**: Implement techniques to make model predictions more interpretable to medical practitioners.
5. **Deployment**: Create a web application for easy access and usage by healthcare professionals.
6. **Multi-class Classification**: Extend the model to classify different types of brain tumors.
7. **Ensemble Methods**: Explore ensemble techniques to potentially improve overall performance.

## 📊 Data Visualization

The notebook includes various visualizations, including:
- Distribution of tumorous vs. non-tumorous images
- Sample preprocessed images
- Training and validation accuracy/loss curves

## 🛠 Technologies Used

- Python
- TensorFlow / Keras
- OpenCV
- Matplotlib
- NumPy
- Pandas
