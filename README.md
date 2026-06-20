# 🗃️ Large-Scale Image Preprocessing Pipeline

A high-performance image preprocessing pipeline built to handle **500,000+ images** efficiently using Python and OpenCV. Designed to clean, standardize, and prepare massive image datasets for Machine Learning and Computer Vision workflows.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat&logo=python&logoColor=white)

---

## 📌 Overview

Raw image datasets are rarely ready for training. They often contain corrupt files, inconsistent sizes, noise, and format issues — all of which reduce model performance. This pipeline automates the **entire preprocessing workflow** from loading raw images to producing clean, model-ready data at scale.

Built to handle the scale demands of real ML projects — tested on datasets of **500,000+ images**.

---

## ✨ Features

- ✅ Batch processing of **500,000+ images** efficiently
- ✅ Image resizing to target dimensions
- ✅ Pixel normalization (0–1 range)
- ✅ Grayscale conversion & color space handling (BGR → RGB)
- ✅ Noise reduction and Gaussian filtering
- ✅ Corrupt and unreadable image detection & removal
- ✅ Duplicate image handling
- ✅ Memory-efficient processing using OpenCV batch operations
- ✅ Visual progress tracking with Matplotlib

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python | Core scripting |
| OpenCV | Image loading, resizing, filtering, color conversion |
| NumPy | Array manipulation & normalization |
| Matplotlib | Visualization of preprocessing results |
| Jupyter Notebook | Interactive development & step-by-step walkthrough |

---

## 📂 Project Structure

```
Preprocessing-Pipeline/
│
├── preprocessing-pipeline.ipynb   # Full pipeline — all steps documented
└── README.md
```

---

## 🧠 Pipeline Steps

```
Raw Image Dataset (500,000+ images)
            │
            ▼
    1. Load & Validate
       (detect & skip corrupt/unreadable files)
            │
            ▼
    2. Resize to Target Dimensions
       (standardize all images to same size)
            │
            ▼
    3. Color Space Conversion
       (BGR → RGB, or Grayscale as needed)
            │
            ▼
    4. Noise Reduction
       (Gaussian blur / median filtering)
            │
            ▼
    5. Pixel Normalization
       (scale values to 0–1 range)
            │
            ▼
    6. Export Processed Dataset
       (save cleaned images / numpy arrays)
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/HasnainSherazi/Preprocessing-Pipeline.git
cd Preprocessing-Pipeline
```

### 2. Install dependencies

```bash
pip install opencv-python numpy matplotlib jupyter
```

### 3. Open the notebook

```bash
jupyter notebook preprocessing-pipeline.ipynb
```

### 4. Set your dataset path

Inside the notebook, update the dataset path variable to point to your image folder:

```python
DATASET_PATH = "path/to/your/images/"
TARGET_SIZE = (224, 224)  # adjust to your model's input size
```

Then run all cells to process your dataset.

---

## 📊 Performance

| Metric | Value |
|---|---|
| Dataset Size Tested | 500,000+ images |
| Processing Approach | Batch-wise OpenCV operations |
| Memory Strategy | Efficient buffered loading |
| Output Format | Processed images / NumPy arrays |

---

## 🔮 Future Improvements

- [ ] Add multiprocessing support for even faster throughput
- [ ] Support for data augmentation (flip, rotate, crop)
- [ ] Export to TFRecord / HDF5 format for TensorFlow pipelines
- [ ] Add a CLI interface for non-notebook use
- [ ] Progress bar integration with `tqdm`

---

## 👤 Author

**Syed Muhammad Hasnain Sherazi**
AI Undergraduate @ CUST, Islamabad

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/syed-muhammad-hasnain-sherazi)
[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat&logo=huggingface&logoColor=black)](https://huggingface.co/HasnainSherazi)
[![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=flat&logo=kaggle&logoColor=white)](https://www.kaggle.com/ssyyeedd14)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/HasnainSherazi)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
