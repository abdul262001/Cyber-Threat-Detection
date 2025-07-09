# 🚨 Cyber Threat Detection Based on Artificial Neural Networks Using Event Profiles

This project is an implementation of **AI-powered threat detection** using event profiling from system/network logs. It combines classical machine learning models and advanced deep learning architectures like **CNN** and **LSTM** to identify potential cyber threats. The system is designed with a GUI to facilitate easier use for demonstrations and testing.

---

## 🧠 Project Overview

The system implements an **AI-SIEM (Artificial Intelligence–Security Information and Event Management)** framework that:

* Parses raw event logs (e.g., from KDD dataset)
* Converts them into TF-IDF event vectors
* Trains and evaluates models like:

  * 🔵 **LSTM (Long Short-Term Memory)**
  * 🔵 **CNN (Convolutional Neural Network)**
  * 🟢 **SVM, KNN, Decision Tree, Random Forest, Naïve Bayes**

It compares the models based on **Accuracy**, **Precision**, **Recall**, and **F-Measure**.

---

## 📁 Project Structure

| File / Folder             | Description                                                               |
| ------------------------- | ------------------------------------------------------------------------- |
| `CyberThreatDetection.py` | Main GUI application to run training and evaluation using ML/DL models    |
| `test.py`                 | SVM classifier in a minimal test setup for quick results                  |
| `run.bat`                 | Batch script to launch the GUI application                                |
| `datasets/`               | Folder expected to contain your dataset CSV files (e.g., `kdd_train.csv`) |
| `SCREENSHOTS.docx`        | Step-by-step user guide with screenshots                                  |
| `DOCUMENT.rar`            | Contains project documentation and possibly a detailed report             |
| `SOURCE CODE.rar`         | Contains all source files in compressed form                              |

---

## 🛠️ Setup Instructions

### 1. 🧑‍💻 Requirements

* Python 3.x
* Libraries:

  ```bash
  pip install numpy pandas scikit-learn keras matplotlib
  ```

### 2. 💻 Running the Project

1. **Extract** all files into a single folder
2. Place your dataset (e.g., `kdd_train.csv`) inside a folder named `datasets/`
3. Double-click on `run.bat` **or** run the GUI manually:

   ```bash
   python CyberThreatDetection.py
   ```

---

## 📊 Features & Workflow

1. **Upload Dataset** – Loads the CSV and encodes labels.
2. **TF-IDF Vectorization** – Transforms textual features into TF-IDF weighted vectors.
3. **Event Vector Creation** – Splits the dataset into train/test sets.
4. **Neural Network Profiling** – Trains and evaluates LSTM and CNN models.
5. **Run Classifiers** – Supports SVM, KNN, Decision Tree, Random Forest, Naïve Bayes.
6. **Comparison Graphs** – Displays bar charts for Accuracy, Precision, Recall, and F-Measure.

---

## 📈 Sample Results

* **CNN Accuracy**: \~99%
* **LSTM Accuracy**: \~94%
* **Best Precision**: CNN
* **Best Recall**: LSTM

Detailed screenshots and results can be found in [`SCREENSHOTS.docx`](./SCREENSHOTS.docx).

---

## 📚 Dataset

Tested on the **KDD Cup 1999** dataset (`kdd_train.csv`).

* Contains 9999 labeled network activity records
* Labels are transformed for binary/multi-class classification

---

## 📸 Screenshots

See the [`SCREENSHOTS.docx`](./SCREENSHOTS.docx) for a complete guide with visuals:

* Uploading dataset
* Running algorithms
* Graph results

---

## 📌 Future Improvements

* Integrate real-time streaming event processing
* Expand dataset compatibility
* Convert GUI to a web dashboard

