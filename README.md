# 🖼️ Deep Learning UTS – Image Dataset Preprocessing  

## 📌 Project Overview  
The goal was to analyze and preprocess an **image dataset (Dataset 2B)** for use in computer vision tasks.  

The dataset contains multiple classes of images organized into **train** and **test** folders. The notebook explores dataset structure, image quality, and performs preprocessing to prepare the data for deep learning models.  

---

## 🔎 Steps Performed  

### 1. **Dataset Extraction & Setup**  
- Mounted Google Drive and extracted `Dataset 2B.zip`.  
- Inspected folder structure: `train/` and `test/` directories, each containing subfolders for classes.  

### 2. **Dataset Exploration**  
- Counted number of images per class in both train and test sets.  
- Visualized class distribution using bar charts → checked for **class imbalance**.  
- Inspected image dimensions and aspect ratios → checked consistency.  

### 3. **Image Quality Checks**  
- Looped through training images to record **width, height, and aspect ratio**.  
- Identified variations in resolution and potential problematic images.  
- Detected a few **corrupted/unreadable images** (logged in `errors`).  

### 4. **Data Preprocessing Setup**  
- Used **ImageDataGenerator** (Keras) for preprocessing pipeline:  
  - Rescaling pixel values.  
  - Potential augmentation (rotation, flipping, zoom, etc. if applied later).  
- Prepared dataset to be split into **train/test sets** with consistent input size.  

---

## 📊 Key Insights  
- Dataset is organized properly into `train` and `test` with class subfolders.  
- Some imbalance between classes (visualized in bar plot).  
- Image sizes vary across dataset → resizing required for CNN input.  
- A few corrupted images found and skipped during loading.  

---

## ✅ Conclusion  
- The notebook successfully **prepared Dataset 2B** for deep learning by analyzing distribution, cleaning corrupted files, and checking image dimensions.  
- This preprocessing ensures the dataset is ready for training **Convolutional Neural Networks (CNNs)** or other image classification models.  
