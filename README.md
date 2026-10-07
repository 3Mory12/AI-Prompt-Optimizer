# 🚀 [Tips Hindawi](https://www.tipshindawi.com/) Internship (August–October) 2026

> 🎓 This project was built during the [ **Tips Hindawi** ](https://www.tipshindawi.com/) **Internship (August–October) 2026**.

## 👤 Participant

| Field            | Value                                |
| ---------------- | ------------------------------------ |
| Full Name        | *Omar Ayman Mohamed Khalifa*                     |
| Project Name     | AI Prompt Optimizer                  |
| GitHub Username  | *3Mory12*               |
| Internship Batch | August–October 2026                  |
| Training Program | Large Language Models (LLMs) Program |
| Organization     | [**Edrak for Ai**](https://edrak4ai.com/en)                         |

---

# 📖 Project Overview

**AI Prompt Optimizer** takes a short, vague prompt (for example, *"Write an advertisement."*) and turns it into a clear, professional, structured prompt using an LLM.

The project is a small educational demo of how three ideas work together:

**Prompt Engineering + LLM + Pydantic Structured Output**

```text
User Input → LLM → Prompt Analysis & Optimization → Structured Output Parser (Pydantic) → Final Optimized Prompt
```

A carefully written system prompt tells the LLM to act as a prompt engineer. A Pydantic schema forces the answer into a fixed structure, so the result is always predictable instead of free-form text.

---

# ✨ Features

* Turns a simple prompt into a complete, professional prompt while keeping the user's original intent.
* Returns a structured result with six fields: **Original Prompt, Improved Prompt, Role, Context, Constraints, Expected Output**.
* Uses **Pydantic** and the LLM's structured output feature, not free-form text parsing.
* Clean web interface built with **Gradio** (input card, result card, one-click examples, copy button, empty-input handling).
* The whole project lives in a single, beginner-friendly Jupyter Notebook.

---

# 🛠️ Technologies Used

* **Python 3**
* **Jupyter Notebook** (VS Code / JupyterLab / Colab)
* **OpenAI Python SDK** (used with Groq's OpenAI-compatible API; model: `openai/gpt-oss-20b`)
* **Pydantic**: output schema and validation
* **Gradio**: web interface

---

# ⚙️ Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/<3Mory12>/<AI-Prompt-Optimizer>.git
   cd <AI-Prompt-Optimizer>
   ```

2. Install the requirements:

   ```bash
   pip install openai pydantic gradio
   ```

3. Get an API key from [Groq](https://console.groq.com/keys) (free tier available).

   The notebook asks you to paste the key when you run the setup cell, so it is never saved in the file. You can also set it as an environment variable:

   * Windows (PowerShell): `$env:GROQ_API_KEY="your-key"`
   * Mac / Linux: `export GROQ_API_KEY="your-key"`

> Want to use OpenAI instead? In the setup cell, remove the `base_url` line, set `MODEL_NAME = "gpt-4o-mini"`, and use your OpenAI key.

> ⚠️ Never commit a real API key to GitHub.

---

# 🚀 Usage

1. Open `ai-prompt-optimizer.ipynb` in VS Code, JupyterLab, or Google Colab.
2. Run the cells from top to bottom. Paste your API key when asked.
3. Optimize a prompt in code:

   ```python
   result = optimize_prompt("Write an advertisement.")
   show_result(result)
   ```

4. Or run the last cell to launch the **Gradio web app**, then open the local link (or the temporary public link) in your browser:
   * Type a simple prompt, or click one of the examples.
   * Click **✨ Optimize Prompt**.
   * Read the Improved Prompt, Role, Context, Constraints and Expected Output in separate boxes.

---

# 📸 Demo

<!-- Add your screenshot or GIF here, for example: -->
<!-- ![App screenshot](images/demo.png) -->

*Add a screenshot of the Gradio app here.*

---

# 📈 Results

Example input:

```text
Write an advertisement.
```

Example output:

| Field | Result |
| ----- | ------ |
| **Improved Prompt** | Write an advertisement for [product name] targeting [target audience] in [medium] with a tone of [tone]. The ad should be no more than [word limit] words and include a clear call to action. |
| **Role** | An experienced copywriter |
| **Context** | This ad will be displayed on social media platforms. |
| **Constraints** | No more than 50 words · Use a friendly tone · Include a call to action |
| **Expected Output** | A single paragraph of advertising copy, no more than 50 words, with a clear call to action. |

The project demonstrates a complete, working pipeline from a vague prompt to a validated, structured result. The system prompt was refined after testing so the model avoids inventing unnecessary requirements and keeps the fields consistent with each other.

---

# 🔮 Future Improvements

* Let the user choose the model or provider from the interface.
* Add a "Copy as one full prompt" button that merges all fields into a single prompt.
* Support more languages (for example, Arabic prompts).

---

# 📚 About the Internship

This project was developed as part of the [**Tips Hindawi**](https://www.tipshindawi.com/) **Internship (August–October) 2026**, and it will be showcased on the official [Tips Hindawi](https://www.tipshindawi.com/) website.

[Tips Hindawi](https://www.tipshindawi.com/) is the internships department of [**Edrak for Ai**](https://edrak4ai.com/en), and the internship encourages participants to build real-world projects, apply practical skills, and showcase their work through GitHub.

For more information about the internship, training programs, and upcoming batches, visit the official [Tips Hindawi](https://www.tipshindawi.com/) website.

---

# 📄 License

This project is shared for educational and portfolio purposes.
