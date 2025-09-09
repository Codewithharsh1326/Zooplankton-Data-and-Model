# Zooplankton-Data-and-Model

Dataset and model training for SIH. hi

---

## 📥 Download Dataset

You can download the dataset directly using [kagglehub](https://www.kaggle.com/datasets/raghavdharwal/pelgas-bay-of-biscay-zooscan-zooplankton-dataset/data):

```python
import kagglehub

# Download the dataset
path = kagglehub.dataset_download(
    "raghavdharwal/pelgas-bay-of-biscay-zooscan-zooplankton-dataset"
)

print("Path to dataset files:", path)

