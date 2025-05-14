# Facial Expression Recognition 😃📊

This project uses the FER-2013 dataset to classify facial expressions into six emotions: happy, sad, angry, surprise, fear, and neutral using a custom CNN and transfer learning with VGG16.

## Dataset 🗂️

* **FER-2013**: 48x48 grayscale images
* **Classes**: 6 emotions (disgust excluded)
* **Splits**:

  * 26,543 training images
  * 6,955 validation images
  * 1,800 test images
* **Preprocessing**: Removed corrupted images; augmented training data

## Requirements 📦

```bash
pip install numpy matplotlib tensorflow scikit-learn seaborn pillow
```

## Models 🧠

### Baseline CNN 🏗️

* 3 Conv2D layers (32, 64, 128 filters), MaxPooling, Dense layers
* Trained for 30 epochs with Adam optimizer
* Parameters: 1,306,758

### VGG16 Transfer Learning 🚀

* Pre-trained VGG16 model
* Initially frozen, fine-tuned last 4 layers
* Feature extraction: 15 epochs
* Fine-tuning: 10 epochs
* Test Accuracy: 48.78%
* Parameters: 15,110,214 (395,526 trainable initially)

## Usage 🛠️

```bash
git clone https://github.com/your-username/facial-expression-recognition.git
```

1. Organize FER-2013 dataset into `train/`, `validation/`, and `test/` directories
2. Run the Jupyter notebook or Python script, updating dataset paths as needed
3. View class distribution and training curves 📈

## Future Work 🔮

* Experiment with other pre-trained models 🤖
* Address class imbalance ⚖️
* Optimize hyperparameters 🧪
