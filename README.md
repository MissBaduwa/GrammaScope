# 🔍🧠✨ GrammaScope: Intelligent Grammar Error Analyzer for Human Language

Welcome to **GrammaScope**. This project is an advanced Natural Language Processing (NLP) tool for **analyzing, classifying, and visualizing grammatical errors** in user-generated text based on **Part-of-Speech (POS) tagging**. Built with Python, spaCy, and Matplotlib, the system supports CSV exports, detailed error breakdowns, and high-level linguistic analysis — paving the way for intelligent grammar-aware applications.



---
## 🚀 Overview

At its core, Grammascope leverages **POS tagging**, **token alignment**, and **sequence comparison algorithms** to uncover subtle grammatical inconsistencies between a gold-standard (correct) sentence and a user-generated variant. The tool produces:

- ✅ Token-level error detection (insertion, deletion, replacement)
- ✅ POS-based error classification
- ✅ CSV-based structured error exports
- ✅ Visual analytics of error distributions by POS category

Whether you're researching second language acquisition, building intelligent tutoring systems, or prototyping NLP pipelines — Grammascope provides a lightweight, extensible foundation.

---
## 💡 How It Works

Grammascope processes a list of sentence pairs and performs the following:

1. **Tokenization & POS Tagging**: Uses spaCy to assign universal POS tags.
2. **Sequence Alignment**: Applies `difflib.SequenceMatcher` to align tokens between the correct and user sentence.
3. **Edit Operation Detection**:
    - **Insertions**: Words present in user sentence but not in the correct version
    - **Deletions/Omissions**: Words missing in the user sentence
    - **Replacements**: Word substitutions with mismatched POS
4. **Error Logging**: Each mismatch is recorded with associated POS information.
5. **Aggregation**: Errors are grouped by POS tags and exported as:
    - `pos_error_details.csv` (per-token error log)
    - `pos_error_summary.csv` (aggregated error counts by POS type)

6. **Visualization**: POS-tag error frequencies are plotted to reveal common grammatical issues.


## 🧠 Features at a Glance

- ✅ POS tagging using **spaCy**’s fast and accurate NLP pipeline  
- ✅ Detection of 3 core grammatical issues: **replacement, omission, and insertion**
- ✅ Deep linguistic tagging and **classification by POS**
- ✅ Clean, exportable reports in **CSV** format (for analysis, training, or feedback)
- ✅ Graphical error visualizations using `matplotlib`
- ✅ Scalable and dashboard-ready (web dashboard coming soon!)

---

## 📦 Sample Dataset

GrammaScope works with a simple but structured dataset of dictation comparisons:

```json
[
  {
    "id": 1,
    "correct": "The quick brown fox jumps over the lazy dog.",
    "user": "The quick fox jump over a lazy dog."
  }
]
```
## ⚙️ Tech Stack
- 🧠 spaCy – POS tagging and linguistic features
- 📊 Matplotlib – For generating insightful visualizations
- 📁 Difflib – Smart sequence matching of sentences
- 📄 CSV – Export logs for post-analysis
- 🧪 Jupyter Notebook – Friendly development and testing environment
- 🧰 Python 
---
## 📥 Installation
1. Clone the repo:
```
git clone https://github.com/yourusername/grammascope.git
cd grammascope
```
2. Install dependencies:
```
pip install spacy matplotlib
python -m spacy download en_core_web_sm
```
3. Launch Jupyter notebook:
```
jupyter notebook
```
4. Open grammar_analysis.ipynb and run all cells to process the dataset and view results.

---
## 💼 Use Cases
- 📚 Language education platforms (give real-time feedback to students)
- 🎤 Speech-to-text training (identify system transcription gaps)
- 🤖 Grammar-aware chatbots
- 🧪 Research in NLP and human error modeling

---
## 📈 Future Work
- ✅ Streamlit-based web dashboard (in progress)
- 🔜 Integration with speech-to-text modules for automated dictation feedback
- 🔜 Grammar suggestion engines using language models (LLMs like GPT or transformer models)
- 📊 Multi-sentence comparison support
- 🌍 Support for other languages (French, Arabic, Twi?)

---
## 🧑‍💻 Author
Built with ❤️ by **Ama Baduwa Baidoo**

Final-year CS student | NLP enthusiast | Curious technologist

“I believe feedback-driven language learning should be both smart and insightful.”

---
## 📜 License
MIT License – free for personal, academic, and commercial use.

---
## 🌟 Give It a Star!
If this project inspires, teaches, or helps you — don’t forget to ⭐️ the repo!

---
