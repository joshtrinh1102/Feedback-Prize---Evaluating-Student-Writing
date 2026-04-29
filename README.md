Feedback Prize - Evaluating Student Writing
This project focuses on the automated evaluation of student writing using various Natural Language Processing (NLP) architectures, including LSTMs, DeBERTa, and Longformers. The goal is to identify and classify rhetorical and argumentative elements in student essays.

📁 Repository Structure
LSTM_Model.ipynb: Implementation of the Long Short-Term Memory network approach.

DeBERTa_v3_large.ipynb: Implementation using the DeBERTa-v3-large transformer model.

LongFormer.ipynb: Implementation using the Longformer architecture, optimized for long documents.

FeedbackPrize_Report.docx: Comprehensive documentation covering methodology, hyperparameter tuning, and final results.

🚀 Getting Started
Follow these steps to set up the environment and reproduce the results.

Step 1: Data Acquisition & Environment Setup
Download the Dataset: Obtain the competition data from the Kaggle Feedback Prize 2021 page.

Google Colab Setup: * Upload the downloaded dataset to your Google Drive or directly to your Colab session.

Ensure you have a GPU runtime enabled (T4, V100, or A100 recommended for transformer models).

Step 2: Training the Baseline (LSTM)
Run the LSTM_Model.ipynb notebook. This establishes the baseline performance for the sequence tagging task using a recurrent architecture.

Step 3: Training DeBERTa
Run the DeBERTa_v3_large.ipynb notebook. This model utilizes advanced attention mechanisms and pre-training techniques to improve classification accuracy on student segments.

Step 4: Training Longformer
Run the LongFormer.ipynb notebook. This architecture is specifically chosen to handle the full length of student essays without the typical token limits of standard transformers.

📝 Methodology
For a deep dive into the experimental design, feature engineering, and model architectures used in this project, please refer to the FeedbackPrize_Report.docx file included in this repository.

📊 Evaluation & Inference
Once the models are trained or the weights are provided:

Load Weights: Utilize the load_state_dict or equivalent functions within the notebooks to load the .bin or .pt model files.

Run Evaluation: Execute the final cells in each notebook to generate evaluation metrics (e.g., F1-score) on the validation or test sets.

Inference: You can use the provided inference pipelines to predict argumentative elements on new, raw text samples.

🛠 Tech Stack
Language: Python

Libraries: PyTorch, Hugging Face Transformers, Pandas, NumPy

Environment: Google Colab / Kaggle Notebooks
