
# CNN Depth Analysis on CIFAR-10

This project investigates how the **depth of a Convolutional Neural Network (CNN)** affects its ability to classify images from the CIFAR-10 dataset. We compare three models — shallow, mid-depth, and deep CNNs — and evaluate how increasing the number of convolutional layers influences performance.

---

## Summary

We train and evaluate the following models:

| Model       | Convolutional Layers | Train Acc | Val Acc | Comment              |
|-------------|----------------------|-----------|---------|-----------------------|
| ShallowCNN  | 2                    | ~81.67%   | ~71.92% | Underfits             |
| MidCNN      | 4                    | ~85.61%   | ~75.41% | Best generalization   |
| DeepCNN     | 6                    | ~79.15%   | ~74.09% | Slight overfitting    |

---

## Project Structure

```
cnn-depth-analysis/
│
├── models/                  # CNN architecture definitions
│   ├── shallow_cnn.py
│   ├── mid_cnn.py
│   └── deep_cnn.py
│
├── utils/                   # Dataset and transformation utilities
│   └── dataset_loader.py
│
├── scripts/                 # Training and evaluation scripts
│   ├── train.py
│   └── evaluate.py
│
├── notebooks/               # Jupyter notebooks for experiments
│   └── cnn_depth_comparison.ipynb
│
├── outputs/                 # Plots and saved results
│   ├── accuracy_plot.png
│   └── loss_plot.png
│
├── requirements.txt         # Python package dependencies
├── tutorial_report.pdf      # Final written report (optional)
├── LICENSE                  # Open source license
└── README.md                # This file
```

---

## Dataset

We use the CIFAR-10 dataset from [https://www.cs.toronto.edu/~kriz/cifar.html](https://www.cs.toronto.edu/~kriz/cifar.html), consisting of 60,000 32x32 RGB images in 10 categories.

---

## How to Run

### 1. Clone this repository

```bash
git clone https://github.com/Sumairch1/cnn-depth-analysis.git
cd cnn-depth-analysis
```

### 2. (Optional) Create a virtual environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Jupyter Notebook

```bash
jupyter notebook notebooks/cnn_depth_comparison.ipynb
```

---

## Output

You will generate:
- Validation accuracy and loss plots
- A trained model comparison
- Performance summary with visual graphs

All visual outputs are saved in the `outputs/` directory.

---

##  License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT). You are free to reuse, modify, and distribute this material with proper attribution.

---

## Author

Developed by Sumair Samad
University of Hertfordshire  
Machine Learning Coursework, 2025
