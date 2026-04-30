# Feedback Prize - Evaluating Student Writing

This project uses NLP architectures (LSTM, DeBERTa, and Longformer) to identify and classify rhetorical elements in student essays.Team Members: Hashim Khan, Sherman LaCost, Josh Trinh
---

## 📁 Repository Structure

* **`LSTM_Model.ipynb`**: Baseline recurrent architecture.
* **`DeBERTa_v3_large.ipynb`**: Advanced transformer-based classification.
* **`LongFormer.ipynb`**: Optimized for long-form document processing.
* **`FeedbackPrize_Report.docx`**: Technical documentation on methodology and results.

---

## 🚀 Getting Started

1.  **Data:** Download the dataset from the [Kaggle Feedback Prize 2021](https://www.kaggle.com/competitions/feedback-prize-2021) competition and upload it to Google Colab.
2.  **Training:** Execute the notebooks in the following order to train the models:
    * `LSTM_Model.ipynb`
    * `DeBERTa_v3_large.ipynb`
    * `LongFormer.ipynb`
3.  **Details:** Refer to **`FeedbackPrize_Report.docx`** for specific hyperparameters and experimental design.

---

## 📊 Evaluation

1.  **Load:** Import pre-trained weights (`.bin` or `.pt`) within each notebook.
2.  **Metrics:** Run the final cells to generate F1-scores and validation performance.
3.  **Inference:** Use the provided pipelines to test the models on new text samples.

---

## 🛠 Tech Stack

* **Frameworks:** PyTorch, Hugging Face Transformers.
* **Data Tools:** Pandas, NumPy.
* **Environment:** Google Colab.
