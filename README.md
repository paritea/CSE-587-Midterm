# CSE-587 Midterm Project

This repository contains the code and experiments for my midterm project in CSE-587. The main focus is on an ablation study of a bidirectional LSTM model for text classification. The final optimized model is implemented in the notebook `cse587-midterm-project-experiment.ipynb`.

## Experiments

The following experiments were conducted:

- **Early Stopping Experiment:**  
  See `early-stop-experiment.ipynb` to observe the impact of early stopping on training. Early stopping was set to monitor validation loss with a patience of 5 epochs, and training halted around 20 epochs when validation performance plateaued.

- **Dropout Study:**  
  To analyze the effect of dropout, I varied the dropout rate across 0.2, 0.4, 0.5, and 0.6. Due to Kaggle's memory limits, these experiments were split into two notebooks:  
  - `dropout-study.ipynb`  
  - `dropout2.ipynb`  
  The results from both notebooks were compiled manually to compare the performance across the four dropout values.

- **BiLSTM Layer Depth Comparison:**  
  I also experimented with the number of BiLSTM layers, comparing models with one layer versus two layers, to understand the impact of network depth on performance. See one-layer-bilstm.ipynb to look at the results of our experiment for 1 layer.

## Steps to Reproduce

1. **Upload Notebooks to Kaggle:**  
   The notebooks are designed to run on Kaggle. Simply upload them to a Kaggle Notebook.

2. **GPU Requirement:**  
   Kaggle’s free GPU (we used two NVIDIA T4 GPUs) is sufficient to run these experiments. Also why we used Kaggle.

3. **Data and Word Vectors:**  
   - **Word Vectors:**  
     Add the [GoogleNews-vectors-negative300](https://www.kaggle.com/datasets/leadbest/googlenewsvectorsnegative300) dataset.
   - **Dataset:**  
     Add the [Bias of US News Media Houses](https://www.kaggle.com/datasets/sushovansaha9/bias-of-us-news-media-houses) dataset.

