# 📃 Panda Resume Critiquer Using DeepSeek DeepSeek V3 0324


**Panda Resume Critiquer** is an AI-powered tool that evaluates resumes using the DeepSeek V3 0324 model. It provides actionable feedback on structure, clarity, and content impact, helping job seekers and recruiters optimize resumes for better results.

![App Screenshot](https://github.com/Ahnuf-Karim-Chowdhury/Panda-Resume-Critiquer-Using-DeepSeek-DeepSeek-V3-0324/blob/main/Images/01_upscayl_5x_realesrgan-x4plus.png?raw=true)

## 🚀 Features

- Upload resumes in **PDF** or **TXT** format.
- Analyze resumes with **DeepSeek V3 0324** via OpenRouter.
- Get feedback on:
  - Clarity and impact of content
  - Presentation of skills
  - Description of experience
  - Tailored improvements based on job role (optional input)
- Easy-to-use **Streamlit** web interface.

---

## 🧠 How It Works

1. **User uploads** their resume.
2. The app extracts and parses the text using `PyPDF2` or directly from `.txt` files.
3. A prompt is crafted with the resume content and (optionally) a target job role.
4. The **DeepSeek V3 0324** model is queried through the OpenRouter API.
5. **AI-generated feedback** is returned in a structured, actionable format.

---

![Panda Resume GIF](https://github.com/Ahnuf-Karim-Chowdhury/Panda-Resume-Critiquer-Using-DeepSeek-DeepSeek-V3-0324/blob/main/Images/Panda%20Resume%20-%202K.gif?raw=true)



## 📦 Dependencies

This project uses the following Python packages:

- `streamlit` – Web UI framework.
- `openai` – OpenRouter client interface.
- `PyPDF2` – Extracts text from PDF resumes.
- `python-dotenv` – Loads environment variables from `.env` file.
- `uv` – Python package manager & runtime (alternative to pip + venv).

### Install with `uv`:

```bash
uv init .
uv add streamlit openai PyPDF2 python-dotenv
```

## 🔧 Setup

1. **Clone this repository**.

2. **Create a `.env` file** in the root directory with your OpenRouter API key:

   ```ini
   API_KEY=your_openrouter_api_key
   ```
3.Install with `uv`
4.Install dependencies :
```bash
uv init .
uv add streamlit openai PyPDF2 python-dotenv
```
5. Run the app using :
   ```bash
   uv run streamlit run main.py
   ```
6.Enjoy.

![Panda Resume Critiquer GIF](https://github.com/Ahnuf-Karim-Chowdhury/Panda-Resume-Critiquer-Using-DeepSeek-DeepSeek-V3-0324/blob/main/Images/Panda_Resume_Cretiquer.gif?raw=true)

## 🖼️ UI Overview

- **Upload Section**: Drop your `.pdf` or `.txt` resume file.
- **Job Role Field** *(optional)*: Input a role you're targeting (e.g., "Software Engineer").
- **Analyze Button**: Starts the AI analysis and displays structured feedback.

---

## 🧠 AI Model

This app uses the **DeepSeek V3 0324** model via **OpenRouter**.

- A **system role prompt** primes the model as an expert HR reviewer.
- Configured with:
  - `temperature = 0.7`
  - `max_tokens = 1000`
- Delivers **balanced**, **specific**, and **actionable** resume feedback.
---
## ✨ Credits

Built with ❤️ using:

- [Streamlit](https://streamlit.io/)
- [OpenRouter](https://openrouter.ai/)
- [DeepSeek](https://deepseek.com/)

