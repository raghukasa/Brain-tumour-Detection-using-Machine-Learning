

# 🧠 Brain Tumor Localization using Deep Q-Networks and Q-Learning

This project leverages **Reinforcement Learning (RL)** techniques—**Q-Learning** and **Deep Q-Networks (DQN)**—to automate the **detection**, **localization**, and **segmentation** of brain tumors in MRI scans. Developed as a final-year B.Tech project at **ICFAI Foundation for Higher Education**, this system provides accurate and interpretable results for medical diagnostics.

---

## 📌 Features

* 🔍 **Binary Classification** of MRI scans into Tumor / No Tumor
* 🎯 **Tumor Localization** using Q-Learning & GridWorld simulation
* 🧩 **Segmentation** of tumor regions highlighted in red
* 📈 High accuracy:

  * Training: **93.10%**
  * Validation: **89.29%**
  * Test: **83.33%**
* 📊 Evaluation Metrics: F1-score, Dice Coefficient, IoU

---

## 🧠 Technologies Used

* **Language:** Python 3.x
* **Frameworks & Libraries:**

  * TensorFlow (Keras)
  * OpenAI Gym
  * NumPy, Pandas
  * Matplotlib, Seaborn
* **Environment:** Google Colab (GPU-enabled)

---

## 🗂️ Dataset

**Brain MRI Images for Brain Tumor Detection**

* Categories: `With Tumor`, `Without Tumor`
* Source: [Kaggle Dataset](https://www.kaggle.com/navoneel/brain-mri-images-for-brain-tumor-detection)

---

## 🏗️ System Architecture

### 🧪 1. Preprocessing

* Resize, Normalize, Augment MRI images

### 🧠 2. Classification

* ResNet50 for binary classification (tumor / no tumor)

### 📍 3. Localization

* Q-Learning to explore the image grid
* DQN for refining tumor position via reward-based learning
* Grid-based movement (down and right) to localize tumor area

### 🔬 4. Segmentation

* Highlight tumor area in red
* Visualize using bounding boxes & overlays

---

## 📊 Model Evaluation

| Metric      | Tumor | No Tumor |
| ----------- | ----- | -------- |
| Precision   | 0.79  | 0.89     |
| Recall      | 0.90  | 0.76     |
| F1-Score    | 0.84  | 0.82     |
| Dice Coeff. | 0.844 | 0.820    |
| IoU (Avg.)  | 0.610 | -        |

---

## 🛠️ How to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/raghukasa/Brain-tumour-Detection-using-Machine-Learning
   ```

2. Open `brain_tumor_rl.ipynb` in **Google Colab**

3. Upload the MRI dataset and follow the step-by-step execution cells:

   * Install dependencies
   * Preprocess data
   * Train Q-Learning agent
   * Train DQN agent
   * Visualize outputs

---

## 🚀 Future Enhancements

* Integrate **3D MRI scan support**
* Combine **multi-modal imaging** (MRI + CT/PET)
* Add **real-time detection** capabilities
* Use **Explainable AI (XAI)** for transparency in clinical settings

---

## 🧑‍💻 Author

**K. Devi Raghu Vara Prasad**
B.Tech CSE, ICFAI Foundation for Higher Education
Mentor: **Dr. Madhusudhan Rao N**

---

## 📚 References

* [Reinforcement Learning: Sutton & Barto](http://incompleteideas.net/book/the-book.html)
* [DQN Nature Paper](https://www.nature.com/articles/nature14236)
* [U-Net for Biomedical Segmentation](https://arxiv.org/abs/1505.04597)

---

Let me know if you'd like a downloadable version or auto-generated version of this `README.md`.
