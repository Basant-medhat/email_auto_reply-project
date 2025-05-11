📘 Project Description
This project builds an Email Auto-Responder using Natural Language Processing (NLP). The goal is to classify customer emails into categories and automatically respond to them using pre-defined templates. Various machine learning models like SVM, RNN, and LSTM were used to classify the email intent and generate appropriate responses.

🚀 Approach Taken
🔁 Cross-Validation
Implemented 5-Fold Cross-Validation using KFold from sklearn.model_selection. For each fold:

Model is trained and evaluated.

Accuracy and F1 Score are recorded.

Final metrics are averaged across all folds to ensure model stability and generalization.

🧰 Preprocessing
Text Normalization: Lowercased all the text to reduce vocabulary size.

Tokenization: Split text into tokens for further processing.

Stopwords Removal: Removed common, irrelevant words (e.g., "the", "is") to improve model accuracy.

TF-IDF Vectorization: Converted the email text into numerical format using TfidfVectorizer.

🧠 Models Used
SVM: Trained using sklearn.svm.SVC, with TF-IDF features.

RNN: Recurrent Neural Network with Embedding and Dense layers for sequence prediction.

LSTM: Long Short-Term Memory network for better handling of long-range dependencies in text.

📊 Model Performance
SVM Model:
Accuracy: 0.95

F1-Score: 0.93 (weighted average)

Precision: 0.91

Recall: 0.95

This model was highly efficient with predefined responses, but struggles with rare classes like "if possible."

RNN Model:
Accuracy: 0.95

F1-Score: 0.98 (weighted average)

Precision: 0.95

Recall: 1.00

RNN performed exceptionally well for most intents, but still needs more fine-tuning for rare cases.

LSTM Model:
Accuracy: 0.95

F1-Score: 0.93 (weighted average)

Precision: 0.91

Recall: 0.95
