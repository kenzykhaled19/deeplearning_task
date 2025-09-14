# Deep Learning Assignment

This repository contains my work on a deep learning assignment covering data preparation, optimizers, batch sizes, regularization, and early stopping. The project demonstrates practical experiments and comparisons across different training setups.

---

## 📂 Project Structure

* **Part 0: Data Preparation**
* **Part 1: Optimizers**
* **Part 2: Batch Size**
* **Part 3: Overfitting and Regularization**
* **Part 4: Early Stopping**
* **Part 5: Reflection**

---

## Part 0: Data Preparation

1. Loaded the dataset into a DataFrame.
2. Split data into **training (70%)**, **validation (15%)**, and **test (15%)** sets.
3. Applied preprocessing: encoding categorical features and scaling numerical features.
4. Reported results on: **training accuracy, validation accuracy, and test accuracy**.
5. Compared all methods across splits at the end.

---

## Part 1: Optimizers

* Trained the same neural network with:

  * **Stochastic Gradient Descent (SGD)**
  * **SGD with Momentum**
  * **Adam**
* Compared training and validation accuracy.
* Observed which optimizer converges the fastest and which generalizes best.
* Explained why **Adam** often outperforms plain SGD.

---

## Part 2: Batch Size

* Trained the model with batch sizes: **1, 32, 128, 1024**.
* Compared:

  * Training speed
  * Validation accuracy
  * Test accuracy
  * Generalization ability
* Identified which batch size led to **noisiest gradients** and which generalized better (smaller batch sizes typically generalize better).

---

## Part 3: Overfitting and Regularization

* Trained a large neural network with many parameters.
* Observed overfitting: training accuracy >> validation accuracy.
* Applied regularization methods:

  * **L2 Regularization**
  * **Dropout**
* Compared validation accuracy before and after applying regularization.
* Highlighted which regularization method reduced overfitting more effectively.

---

## Part 4: Early Stopping

* Trained the model for many epochs without early stopping and plotted train/validation/test curves.
* Trained again with **early stopping** (monitoring validation loss).
* Compared number of epochs and final performance.
* Explained how early stopping prevents overfitting and saves training time.

---

## Part 5: Reflection

### Key Learnings

* **Optimizers**: Adam is generally the fastest and most stable, though momentum helps SGD.
* **Batch Size**: Smaller batches generalize better but are noisier; large batches converge smoothly but risk poor generalization.
* **Regularization**: Both L2 and Dropout reduce overfitting, with dropout often being more effective.
* **Early Stopping**: A practical technique to halt training before overfitting starts.
* **Data Splits**: Essential to keep a separate validation and test set for fair evaluation.

### My Preferred Setup for New Tabular Data

* **Optimizer**: Adam (fast convergence, good performance).
* **Batch Size**: 32 or 64 (balance between speed and generalization).
* **Regularization**: Dropout + L2 if needed.
* **Early Stopping**: Always enable with patience \~5 epochs.
* **Data Split**: 70% train, 15% validation, 15% test.

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/USERNAME/REPO.git
   cd REPO
   ```
2. Open the notebook in **Google Colab** or **Jupyter Notebook**.
3. Run all cells to reproduce results.

---

## 📊 Results

All experimental results (training, validation, test accuracies) are included in the notebooks with plots and comparisons.

---

## 📝 Author

Created by **Kenzy khaled Mahmoud** as part of a deep learning assignment.
