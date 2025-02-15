# 🐍 Multilingual NER with Transformers

## 📝 Description
This Python script demonstrates **multilingual Named Entity Recognition (NER)** using transformer models like **XLM-RoBERTa**. It fine-tunes the model on the **PAN-X dataset** (German, French, Italian, and English) and evaluates its performance across languages. The script also includes zero-shot transfer learning and fine-tuning on multiple languages.

## 🛠️ Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/navidfalah/multilingual-ner-transformers.git
   cd multilingual-ner-transformers
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Install additional libraries:
   ```bash
   pip install datasets seqeval transformers
   ```

## 🚀 Usage
1. Run the script:
   ```bash
   python multilingual_ner_transformers.py
   ```
2. The script will:
   - Load and preprocess the PAN-X dataset for multiple languages.
   - Fine-tune the XLM-RoBERTa model on the German subset.
   - Evaluate the model on other languages using zero-shot transfer learning.
   - Fine-tune on multiple languages and evaluate performance.

## 📂 File Structure
```
multilingual-ner-transformers/
├── multilingual_ner_transformers.py  # Main script
├── README.md                         # This file
├── requirements.txt                  # Dependencies
└── data/                             # (Optional) Data folder for local inputs
```

## 🧩 Key Features
- **Multilingual NER**:
  - Fine-tune XLM-RoBERTa on the PAN-X dataset for German, French, Italian, and English.
  - Evaluate zero-shot transfer learning across languages.
- **Model Training**:
  - Fine-tune on individual languages and combinations of languages.
  - Use custom token classification heads for NER.
- **Evaluation**:
  - Calculate F1 scores for NER tasks.
  - Generate confusion matrices for error analysis.

## 📊 Example Outputs
1. **F1 Scores**:
   - German: 0.85
   - French: 0.78
   - Italian: 0.72
   - English: 0.80
2. **Confusion Matrix**:
   - Visualize normalized confusion matrix for NER predictions.

## 🤖 Models Used
- **XLM-RoBERTa**: A multilingual transformer model for NER tasks.

## 📈 Performance Metrics
- **F1 Score**: Measures the accuracy of NER predictions.
- **Confusion Matrix**: Visualizes prediction errors.

## 🛠️ Dependencies
- Python 3.x
- Libraries:
  - `torch`, `transformers`
  - `datasets`, `seqeval`
  - `numpy`, `pandas`, `matplotlib`

## 🤝 Contributing
1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature`.
3. Commit your changes: `git commit -m "Add your feature"`.
4. Push to the branch: `git push origin feature/your-feature`.
5. Open a pull request.

## 📜 License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 👤 Author
- **Name**: Navid Falah
- **GitHub**: [navidfalah](https://github.com/navidfalah)
- **Email**: navid.falah7@gmail.com
