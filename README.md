# Building-AI-Browser-Agents

# 🎓 AI-Powered Learning Path Generator

This project generates structured learning paths using OpenAI's GPT and live web scraping from [DeepLearning.AI](https://www.deeplearning.ai/courses). It comes in two flavors:
---

![Gradio Interface Demo](assets/output.gif)

## 📦 Versions

- 🧩 `simple_agent.ipynb`: Gradio-powered interactive app for real-time course recommendations.
- 📒 `autonomous_agent.ipynb`: A step-by-step notebook implementing logic with chain-of-thought reasoning.
- 🔁 `MCTS and AgentQ.ipynb`: (Experimental) Integrates Monte Carlo Tree Search and decision-based agents for autonomous planning (WIP).

---

## 🚀 Features

✅ Enter any AI-related topic (e.g., "RAG", "LangChain", "NLP")  
✅ Uses live data from DeepLearning.AI  
✅ GPT filters and structures raw course text  
✅ Automatically classifies courses: Beginner / Intermediate / Advanced  
✅ Clean Markdown outputs  
✅ Visualized roadmaps or Gradio UI

---

## 📁 Project Structure

```bash
├── simple_agent.ipynb           # 🧩 Gradio app + web scraper + GPT integration
├── autonomous_agent.ipynb       # 📒 Visual logic and experimentation
├── MCTS and AgentQ.ipynb        # 🔁 Planning agent framework (MCTS logic)
├── README.md                    # 📘 This file

---

### 🖥️ Display  

- **Simple Agent**: Returns Markdown-formatted course roadmap in a **Gradio web interface**  
- **Autonomous Agent**: Displays structured results in notebook cells and/or visualized using the `visualizeCourses()` function (if enabled)
- **MCTS Agent (Experimental)**: Integrates decision-making via search-based policies to extend automation.


## 🌟 Future Roadmap

- [ ] Add PDF export of generated course roadmap  
- [ ] Integrate additional course providers (Coursera, Udemy, edX)  
- [ ] Extend MCTS Agent to autonomous decision loops  
- [ ] Add roadmap feedback loop with user scoring  

