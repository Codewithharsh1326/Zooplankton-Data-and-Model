# Zooplankton-Data-and-Model

Dataset and model training for SIH.

---

## 📥 Download Dataset

You can download the dataset directly using [kagglehub](https://github.com/Kaggle/kagglehub):

```python
import kagglehub

# Download the dataset
path = kagglehub.dataset_download(
    "raghavdharwal/pelgas-bay-of-biscay-zooscan-zooplankton-dataset"
)

print("Path to dataset files:", path)

