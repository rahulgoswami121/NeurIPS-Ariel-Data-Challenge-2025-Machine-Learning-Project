# NeurIPS Ariel Data Challenge 2025 – Machine Learning Project

This repository contains my solution and exploration for the **NeurIPS Ariel Data Challenge 2025**, developed in a Kaggle notebook environment with **internet disabled**. The notebook focuses on data preprocessing, feature engineering, model experimentation, and parallel processing setups required for the challenge.

---

## 📌 Project Overview

The objective of this project is to build machine learning models that can effectively learn from the provided competition dataset. The notebook is structured to support efficient data loading, modular experimentation, and reproducibility.

Since the challenge requires working in a restricted environment (such as Kaggle without internet), the project includes approaches to installing offline packages, handling large datasets, and ensuring smooth execution.

---

## 📂 Repository Structure

```plaintext
NeurIPS-Ariel-Data-Challenge-2025-Machine-Learning-Project/
│
├── notebook.ipynb               # Primary Kaggle notebook
├── README.md                    # Project documentation
└── input/                       # Offline wheels or dataset references (if any)
```

---

## ⚙️ Key Features of the Notebook

### 1. **Offline Package Installation**

Kaggle does not allow internet access by default in competitions, so external libraries such as **pqdm** (for parallel processing) must be installed using local wheels:

```python
!pip install --no-index --find-links=/kaggle/input/ariel-2024-pqdm pqdm
```

The notebook documents the expected file locations and troubleshooting steps.

### 2. **Data Handling**

- Efficient loading using `pandas`
- Memory optimization where needed
- Exploratory checks on dataset size, types, and missing values

### 3. **Machine Learning Pipeline**

- Feature preprocessing
- Custom model architectures using **PyTorch**
- Training loop setup with GPU compatibility
- Validation strategies

### 4. **Parallel Processing Support**

The notebook uses:

- `multiprocessing`
- `pqdm` for parallelized map operations This significantly speeds up compute-heavy preprocessing.

### 5. **Modular Code Structure**

The notebook separates concerns like:

- Data loading
- Feature engineering
- Model definition
- Training & evaluation making it maintainable and easy to extend.

---

## 📊 Technologies Used

- **Python 3**
- **Pandas**, **NumPy**
- **PyTorch**
- **Multiprocessing**, **pqdm**
- Kaggle notebook runtime (CPU/GPU)

---

## 🚀 How to Run

1. Open the Kaggle notebook.
2. Upload or mount the required offline package folder:
   - `ariel-2024-pqdm/` containing the `pqdm` wheel file.
3. Run the notebook cells sequentially.
4. Modify parameters in the training section to experiment with models.

---

## 📝 Notes

- This notebook is a work in progress as part of the competition.
- Further experiments, models, and results will be added.

---

## 📧 Contact

If you want to discuss this project or collaborate, feel free to reach out: **Rahul Goswami**\
GitHub: [rahulgoswami121](https://github.com/rahulgoswami121)

---

