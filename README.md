# 🚀 NLP_Sentence_Form_Classification

An NLP project that uses a fine-tuned Distil-BERT model to recognize abbreviations and their corresponding long forms in sentences. The project includes model training, deployment on Hugging Face, API integration, stress testing, and a user-friendly Streamlit interface.

## 📖 Table of Contents

- [Introduction]
- [Features]
- [Installation]
- [Usage]
- [Model Training]
- [Model Deployment]
- [Testing]
- [Interface]
- [License]
- [Acknowledgements]

## 🌟 Introduction

This project aims to deploy a Natural Language Processing (NLP) model capable of recognizing abbreviations and their long forms within sentences. The best-performing model, after extensive experimentation, was a fine-tuned Distil-BERT model, optimized for both performance and computational cost.

## ✨ Features

- **Fine-tuned Distil-BERT Model**: Trained on the PLOD-CW dataset to accurately identify abbreviations and long forms.
- **Hugging Face Integration**: Model uploaded to Hugging Face for easy deployment and API access.
- **Stress Testing**: Tested API limits using `Testing.ipynb` notebook.
- **Streamlit Interface**: User-friendly web app allowing users to input sentences and receive analysis.
  
## 🛠️ Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/MaxNardone/NLP_Sentence_Form_Classification.git
   cd NLP_Sentence_Form_Classification
   ```
2. **Create a virtual environment**

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the required packages**

   ```bash
   pip install -r requirements.txt
   ```

## 🚀 Usage

### Running the Streamlit App

```bash
streamlit run infer.py
```

### Testing the Model via Hugging Face API

Refer to the `Testing.ipynb` notebook for examples on how to call the model using Hugging Face's API and perform stress testing.

## 📚 Model Training

Multiple NLP transformer models were initially trained with various configurations. The Distil-BERT model fine-tuned with the PLOD-CW dataset provided the best balance between performance and computational cost.

## 🌐 Model Deployment

The trained Distil-BERT model was uploaded to Hugging Face, providing an accessible API endpoint for inference. This allows for seamless integration with applications and services.

## 🧪 Testing

Stress testing was conducted using the `Testing.ipynb` notebook to evaluate the limits of the Hugging Face API, ensuring reliability and performance under various conditions.

## 🎨 Interface

A Streamlit-based interface was developed, enabling users to input custom or pre-defined sentences. The application analyzes the input to detect abbreviations and long forms, displaying the results in an interactive manner.

## 📄 License

This project is licensed under the MIT License

## 🙏 Acknowledgements

- **Hugging Face** for providing an excellent platform for model deployment.
- **Streamlit** for simplifying the creation of web applications.
- **PLOD-CW Dataset** for the training data.
