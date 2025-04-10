# 🖼️ LeetCode Screenshot OCR Solver

This project automates the process of extracting, solving, and explaining LeetCode-style coding problems from desktop screenshots using OCR and OpenAI GPT models.

---

## 📌 Features

- ✅ Detects open desktop windows and takes a screenshot of a selected one
- 🖼️ Stores screenshots in a dedicated `screen_shots/` folder
- 🔍 Uses Tesseract OCR to extract text from screenshots
- 📝 Saves parsed text into the `parsed_texts/` folder
- 🤖 Sends the extracted text to OpenAI GPT-4o via API to:
  - Identify any LeetCode-style problem
  - Explain the problem in natural language
  - Provide a step-by-step solution with code
- 📄 Saves the GPT-generated solution in Markdown format under `explained_solns/`

---

## 🧠 Example Use Case

Imagine you have a coding challenge open on your screen, and you want:
1. To extract the question text from a screenshot
2. To get an immediate explanation and solution from GPT

This project automates that entire flow.

---
## 📁 Directory Structure
.
├── screen_shots/        # Screenshots of captured windows
├── parsed_texts/        # Raw OCR text extracted from screenshots
├── explained_solns/     # Markdown solutions from OpenAI GPT
├── .env                 # Your OpenAI API key (OPENAI_API_KEY="sk-...")
├── notebook.ipynb       # The Jupyter Notebook to run everything
├── requirements.txt     # Dependency list
└── README.md            # You're here :)

---
## 🛠️ Requirements

Make sure the following tools and Python packages are installed:

- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)  
- Python 3.8+
- Install dependencies:

```bash
pip install -r requirements.txt


