# Setup Guide for Running the Project

## Prerequisites

- Python 3.8 or higher
- Git
- At least 10GB of free disk space (for dataset + features cache)

## Step 1: Clone the Repository

```bash
git clone https://github.com/0duda/UrbanSound8K-Classification.git
cd UrbanSound8K-Classification
```

## Step 2: Create Virtual Environment (Recommended)

### On Windows (PowerShell)
```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
```

### On macOS/Linux
```bash
python -m venv venv
source venv/bin/activate
```

## Step 3: Install Dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

## Step 4: Download UrbanSound8K Dataset

1. Visit [urbansounddataset.org](https://urbansounddataset.org/)
2. Register and download the UrbanSound8K dataset (ZIP file, ~6GB)
3. Extract the ZIP file in the project root directory

Expected structure:
```
UrbanSound8K/
├── audio/
│   ├── fold1/
│   ├── fold2/
│   ├── ...
│   └── fold10/
└── metadata/
    └── UrbanSound8K.csv
```

## Step 5: Launch Jupyter

```bash
jupyter notebook
```

## Running the Notebooks
- `PROJECT.ipynb` - Introduces the project
- `CNN.ipynb` - Train CNN on different feature representations
- `MLP.ipynb` - Train MLP baseline with hyperparameter tuning
- `DEEPFOOL_CNN.ipynb` - Adversarial robustness analysis for CNN
- `DEEPFOOL_MLP.ipynb` - Adversarial robustness analysis for MLP
