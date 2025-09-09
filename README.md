# Zooplankton-Data-and-Model

Dataset and model training for SIH. hi

---

## Clone this Repository

You can clone this repository using:

```bash
git clone https://Codewithharsh1326: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@github.com/Codewithharsh1326/Zooplankton-Data-and-Model.git
cd Zooplankton-Data-and-Model
```

---

## Download Dataset

You can download the dataset directly using [kagglehub](https://www.kaggle.com/datasets/harshpatel1326/zooplankton-dataset-2004-2016/data?select=101141):

But before downloading the data set login using the following code and the information in kaggle.json file:

```python
import kagglehub
kagglehub.login()
```

Then you can download the data set by using following code.

```python
import kagglehub
import os
import shutil

# Download latest version to the default cache location
path = kagglehub.dataset_download("harshpatel1326/zooplankton-dataset-2004-2016")

print("Path to dataset files:", path)

# Define the destination directory
destination_dir = "/content/"

# Create the destination directory if it doesn't exist
os.makedirs(destination_dir, exist_ok=True)

# Move all files and directories from the cache to the destination
for item in os.listdir(path):
    s = os.path.join(path, item)
    d = os.path.join(destination_dir, item)
    if os.path.isdir(s):
        shutil.move(s, d)
    else:
        shutil.move(s, d)

print(f"Files moved to {destination_dir}")
```
---

## Training Data Set

The classes were used to train the model, each containing 10,000 images in total, without any train, validation, or test split.

| Class Name |
|------------|
| nauplii_Crustacea__85116 |
| tail_Appendicularia__85004 |
| Euchaetidae__61986 |
| part_Siphonophorae__92039 |
| nectophore_Diphyidae__84976 |
| Centropagidae__61990 |
| Metridinidae__61982 |
| Cladocera__45036 |
| Noctiluca_Noctilucaceae__58408 |
| fiber_detritus__85076 |

To download the folder contaning the train, test, and validation splited folder with 80, 10, and 10% split, respectively, you can use the following code.

```python
import kagglehub
import os
import shutil

# Download latest version to the default cache location
path = kagglehub.dataset_download("harshpatel1326/zooplankton-model-train-data")

print("Path to dataset files:", path)

# Define the destination directory
destination_dir = "/content/"

# Create the destination directory if it doesn't exist
os.makedirs(destination_dir, exist_ok=True)

# Move all files and directories from the cache to the destination
for item in os.listdir(path):
    s = os.path.join(path, item)
    d = os.path.join(destination_dir, item)
    if os.path.isdir(s):
        shutil.move(s, d)
    else:
        shutil.move(s, d)

print(f"Files moved to {destination_dir}")
```
