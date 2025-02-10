
# **Deepfake Image Detection - Kaggle Competition**

This repository contains the Kaggle notebook and code for the **Deepfake Image Detection** competition. The challenge revolves around detecting whether an image is **AI-generated (deepfake)** or **a real image** using various computer vision techniques.

---

## **Competition Overview**

This is a computer vision competition that allows participants to showcase their skills in exploring vulnerabilities and exploits within the realm of computer vision. The goal is to build models capable of predicting the authenticity of an image—whether it is real or AI-generated.

- **Start Date:** January 26, 2025  
- **End Date:** February 1, 2025  
- **Dataset:** Contains both real and AI-generated images. Labels are represented on a scale of 0 to 1, where:
  - **1** indicates a real image
  - **0** indicates an AI-generated (deepfake) image  
- **Evaluation Metric:** Accuracy, evaluated using **LogLoss**.

---

## **Problem Statement**
In this challenge, you are tasked with predicting whether the given image is:
- **A real image (label = 1)**  
- **An AI-generated image (label = 0)**  

---

## **Dataset Information**
The dataset includes a mix of real and AI-generated images for training and evaluation. The goal is to use machine learning models to differentiate between the two types.

- **Dataset Components:**
  - Training images with corresponding labels
  - Test images for predictions
  - Sample submission format provided

You can download the dataset directly from Kaggle through the competition page.

---

## **Evaluation**
The competition uses **LogLoss** as the evaluation metric. Accuracy is also monitored during training to help identify the model’s generalization performance.

---

## **How to Run the Notebook**

1. **Clone the repository:**
   ```bash
   git clone https://github.com/AnshAggr1303/Deepfake-Imagedetection.git
   cd Deepfake-Imagedetection
   ```

2. **Install the required libraries:**
   You can install dependencies directly using the `requirements.txt` (if provided) or by manually installing the main libraries:
   ```bash
   pip install -r requirements.txt
   ```

   **Key Libraries:**  
   - numpy  
   - pandas  
   - scikit-learn  
   - matplotlib  
   - tensorflow   

3. **Run the notebook locally:**
   Open the Jupyter notebook:
   ```bash
   jupyter notebook deepfake-imagedetection.ipynb
   ```
   
---

## **Submission Guidelines**
To submit predictions for evaluation:
1. Run the notebook and generate the predictions.
2. Prepare the submission file as required by Kaggle (usually `submission.csv`).
3. Submit the file on the Kaggle competition page.

---

## **Evaluation Metric - LogLoss**
The submissions will be evaluated using **LogLoss**, a common metric for binary classification problems.

The formula for LogLoss is:
```
LogLoss = -(1/N) Σ [ y_i * log(ŷ_i) + (1 - y_i) * log(1 - ŷ_i) ]
```
Where:
- N is the number of predictions
- y_i is the actual label
- ŷ_i is the predicted probability of the image being real
  
---

## **Contributing**
Feel free to open an issue or submit a pull request if you have any suggestions or improvements to this repository.

---

## **License**
This project is licensed under the [MIT License](LICENSE) — feel free to use, modify, and distribute it.
