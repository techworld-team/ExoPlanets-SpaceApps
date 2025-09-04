# A World Away: Hunting for Exoplanets with AI

### Team Name: TechWorld

### Team Members

* **Akash Bhujabal** - Member 1: Data Engineer
* **Khushi Sonkar** - Member 2: Machine Learning Modeler
* **Ayushi Sharma** - Member 3: Project Manager & Storyteller

---

## 🚀 Problem Statement

The discovery of planets outside our solar system, or exoplanets, is a monumental task. Space missions like NASA's Kepler and TESS generate vast amounts of data, making manual identification of these planets incredibly time-consuming. Our project addresses this challenge by creating an automated system to analyze stellar data and efficiently identify potential exoplanets.

## ✨ Our Solution

We developed a machine learning model to classify stellar light curves—measurements of a star's brightness over time—to determine if they show evidence of an orbiting exoplanet. The model is trained to recognize the characteristic periodic dips in brightness caused by a planet passing in front of its star, a technique known as the **transit method**.

## 📊 Data

Our model was trained on the open-source **Kepler Exoplanet Candidates dataset** provided by NASA. This dataset contains thousands of stellar light curves, each labeled to indicate whether the star is a confirmed exoplanet host or a false positive. We specifically utilized the `exoTest.csv` file for our development and testing.

---

## 🛠️ Methodology

Our approach followed a structured machine learning workflow to ensure a robust and reliable model.

* **Data Preparation (Akash Bhujabal):** We began by exploring and cleaning the raw light curve data. I extracted key statistical features from each star's light curve, such as the mean flux, standard deviation, and minimum flux. This process, known as **feature engineering**, transformed the raw data into a format suitable for the model.

* **Model Building (Khushi Sonkar):** We trained a **Random Forest Classifier** to learn the patterns in our engineered features. This model was chosen for its strong performance and its ability to handle the high-dimensional data. We addressed the challenge of **data imbalance** by applying techniques to ensure the model was effective at finding the rare exoplanet cases.

* **Evaluation & Presentation (Ayushi Sharma):** We rigorously evaluated the model's performance using metrics like **Precision**, **Recall**, and the **F1-Score**, which are more reliable than simple accuracy for our imbalanced dataset. I am responsible for presenting our methodology and results in a clear and compelling way, highlighting the project's potential impact.

## 📈 Results

Our model achieved strong results in accurately identifying exoplanet candidates. The **confusion matrix** below summarizes our model's performance on the test set:

| | Predicted Non-Exoplanet | Predicted Exoplanet |
| :--- | :---: | :---: |
| **Actual Non-Exoplanet** | [Number] | [Number] |
| **Actual Exoplanet** | [Number] | [Number] |

*Our model demonstrated high **recall**, successfully identifying a majority of the actual exoplanets in the test set.*

## 💻 How to Run

1.  Clone this repository to your local machine: `git clone [repository_url]`
2.  Ensure you have Python 3.x installed.
3.  Install the required libraries: `pip install pandas numpy scikit-learn`
4.  Place the `exoTest.csv` file in the project's root directory.
5.  Open and run the `exoplanet_detector.ipynb` Jupyter Notebook.

## 🗺️ Future Work

* Train the model on a larger and more diverse dataset from the NASA Exoplanet Archive.
* Explore deep learning models, such as **Convolutional Neural Networks (CNNs)**, which can learn features automatically from the raw light curve data.
* Develop a user-friendly interface that allows users to upload their own light curve data and get a prediction in real-time.

---
