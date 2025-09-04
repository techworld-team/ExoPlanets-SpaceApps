# A World Away: Hunting for Exoplanets with AI

### Team Name: [Your Team's Name]

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

* **Model Building (Khushi Sonkar):** We trained a **Random Forest Classifier** to learn the patterns in our engineered features. This model was chosen for its strong
