# 📄 AI Resume Enhancer (Streamlit + OpenAI)

An easy-to-use web app built with [Streamlit](https://streamlit.io/) that lets you upload your resume (PDF or TXT) and receive **AI-powered feedback** tailored to a specific job role or for general job applications.

It uses:
- `PyPDF2` to extract text from PDF resumes
- `python-dotenv` to load your OpenAI API key from a `.env` file
- The official `openai` Python SDK to generate feedback

---

## 🚀 Features

- Upload a PDF or TXT resume.
- Enter a target job role (optional).
- Get structured, actionable feedback on:
  - Content clarity and impact
  - Skills presentation
  - Experience descriptions
  - Specific improvements for the entered job role.

---

## 📦 Requirements

- Python **3.9+**
- An **OpenAI API key** stored in a `.env` file:

## 📦 Python packages used:

- `streamlit`
- `openai`
- `PyPDF2`
- `python-dotenv`

## 🛠️ Installation

1. **Clone this repo**:

git clone https://github.com/Kostiantin/resume_enhancer.git
cd resume_enhancer

2. Create and activate a virtual environment:

python3 -m venv .venv

source .venv/bin/activate   # macOS/Linux

3. Install the dependencies:

pip install --upgrade pip setuptools wheel
pip install streamlit openai PyPDF2 python-dotenv

4. Create a .env file in the project root with your OpenAI key:

OPENAI_API_KEY=sk-xxxxxxx

▶️ Running the App

streamlit run main.py

📝 How It Works

1. The app extracts text from the uploaded PDF or TXT resume.

2. It builds a prompt with the resume text and the optional job role.

3. It sends the prompt to OpenAI’s API to generate feedback.

4. The feedback is displayed in a clear, structured format on the page.