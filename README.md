# Building-AI-Browser-Agents

# 🎓 AI-Powered Learning Path Generator

This project generates structured learning paths using OpenAI's GPT and live web scraping from [DeepLearning.AI](https://www.deeplearning.ai/courses). It comes in two flavors:

- 🧩 `simple_agent.ipynb `: A complete CLI and Gradio-based UI for users to enter a topic and receive course roadmaps.
- 📒 `autonomous_agent.ipynb `: A Jupyter Notebook version for experimenting and visualizing agent logic step by step.

---

## 🚀 Features

✅ Enter a topic like "Python", "RAG", or "NLP"  
✅ Scrape live courses from DeepLearning.AI  
✅ Use GPT to structure course metadata  
✅ Automatically classify into beginner/intermediate/advanced  
✅ Clean Markdown output  
✅ Gradio interface (in Python version)

---

## 📁 Project Structure

```bash
├── simple_agent.ipynb         # 🧩 Full Gradio app + backend logic
├── autonomous_agent.ipynb     # 📒 Notebook for step-by-step interaction
├── helper.py                  # Shared data models (Pydantic)
├── README.md                  # 🔍 This file
├── requirements.txt           # 🔧 Dependencies


## 🧠 How It Works

### 📥 Input  
The user provides a topic of interest (e.g., “Computer Vision”).

---

### 🕸️ Web Scraping  
The app uses `WebScraperAgent` with **Playwright** to extract HTML from [DeepLearning.AI](https://www.deeplearning.ai/courses).

---

### 🧠 GPT Structuring  
The `process_with_llm` function (OpenAI) receives scraping results and filters/structures course data into JSON format for further processing.

---

### 📘 Categorization  
Courses are automatically labeled into three categories:

- **📘 Beginner**: Includes terms like “Intro”, “Getting Started”, etc.  
- **📗 Intermediate**: Default label if no clear beginner/advanced indicators are found  
- **📕 Advanced**: Includes terms like “Advanced”, “Expert”, etc.

---

### 🖥️ Display  

- **Simple Agent**: Returns Markdown-formatted course roadmap in a **Gradio web interface**  
- **Autonomous Agent**: Displays structured results in notebook cells and/or visualized using the `visualizeCourses()` function (if enabled)
