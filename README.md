<h1 align="center">🩺 CNN-Based COVID-19 Diagnostic Support System</h1>

<p align="center">
<strong>Binary Chest X-Ray Image Classification using Deep Learning</strong><br>
Final Project – Intro to Big Data Analytics<br>
Michigan Technological University
</p>

<hr>

<h2>📌 Project Overview</h2>
<p>
This project presents a Convolutional Neural Network (CNN)–based diagnostic support system
designed to classify chest X-ray images into <strong>COVID-19</strong> and <strong>non-COVID</strong> categories.
The system addresses the public health challenge of delayed or limited COVID-19 testing,
particularly in low-resource settings, by leveraging medical imaging and deep learning
to support early triage decisions.
</p>

<p>
The model was trained and evaluated using the publicly available
<strong>COVID-19 Radiography Database</strong> from Kaggle, where multiple non-COVID
conditions (Normal, Viral Pneumonia, Lung Opacity) were consolidated into a single
negative class.
</p>

<hr>

<h2>🎯 Objectives</h2>
<ul>
  <li>Develop a CNN for binary COVID-19 detection from chest X-ray images</li>
  <li>Optimize model performance using regularization and early stopping</li>
  <li>Evaluate model robustness using multiple classification metrics</li>
  <li>Demonstrate applicability as a clinical decision-support tool</li>
</ul>

<hr>

<h2>🧠 Model Architecture</h2>
<ul>
  <li>Input size: <strong>224 × 224</strong> chest X-ray images</li>
  <li>Three convolutional layers with increasing filters (32 → 64 → 128)</li>
  <li>ReLU activations and max-pooling layers</li>
  <li>Flatten layer followed by a dense layer (256 units)</li>
  <li>Dropout for overfitting prevention</li>
  <li>Sigmoid output layer for binary classification</li>
</ul>

<p>
The final model contains approximately <strong>22 million trainable parameters</strong>,
with the majority residing in the fully connected layers, enabling the model to learn
complex radiographic patterns.
</p>

<hr>

<h2>⚙️ Training Configuration</h2>
<ul>
  <li>Optimizer: Adam</li>
  <li>Loss function: Binary Cross-Entropy</li>
  <li>Batch size: 32</li>
  <li>Epochs: 30 (with early stopping)</li>
  <li>Regularization: Dropout, data augmentation</li>
</ul>

<hr>

<h2>📊 Dataset & Preprocessing</h2>
<ul>
  <li>Source: COVID-19 Radiography Database (Kaggle)</li>
  <li>Class distribution (binary):
    <ul>
      <li>COVID-19: 17%</li>
      <li>Non-COVID: 83%</li>
    </ul>
  </li>
  <li>Train / Validation / Test split: 70% / 10% / 20%</li>
  <li>Image augmentation: rotation, flipping, brightness adjustment, zoom</li>
</ul>

<hr>

<h2>📈 Performance Metrics</h2>
<table border="1" cellpadding="6" cellspacing="0">
  <tr>
    <th>Metric</th>
    <th>Score</th>
  </tr>
  <tr><td>Accuracy</td><td>0.98</td></tr>
  <tr><td>Precision</td><td>0.97</td></tr>
  <tr><td>Recall</td><td>0.95</td></tr>
  <tr><td>F1-Score</td><td>0.96</td></tr>
  <tr><td>ROC-AUC</td><td>0.99</td></tr>
</table>

<p>
Training curves demonstrated stable convergence with minimal overfitting.
The ROC curve achieved an AUC of 0.993, and the confusion matrix showed
strong sensitivity and specificity for both classes.
</p>

<hr>

<h2>🧪 Key Results</h2>
<ul>
  <li>High discrimination capability between COVID and non-COVID cases</li>
  <li>Strong recall for COVID-19, reducing false negatives</li>
  <li>Stable training with effective overfitting control</li>
</ul>

<hr>

<h2>⚠️ Limitations & Future Work</h2>
<ul>
  <li>Class imbalance may impact real-world generalizability</li>
  <li>Future work could include transfer learning, explainability (Grad-CAM),
      and multi-class classification</li>
  <li>Clinical validation required before deployment</li>
</ul>

<hr>

<h2>📚 References</h2>
<p>
GoodRx (2020). Over 67 Million Americans Lack Access to COVID-19 Testing.<br>
Kaggle: COVID-19 Radiography Database
</p>

<hr>

<p align="center">
<strong>Author:</strong> Mohammed Abdulai<br>
MS Health Informatics – Michigan Technological University
</p>
