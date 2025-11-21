# 🤖 AI Agent in Python (OpenAI, Anthropic, and Ollama)

This project is based on the excellent tutorial by **Tech With Tim**:  
🎥 [Build an AI Agent From Scratch in Python](https://www.youtube.com/watch?v=bTMPwUgLZf0)

The core idea is to create an intelligent agent in Python, capable of planning, reasoning, and executing tasks autonomously using Large Language Models (LLMs).  
This project has been extended to work with:

- **OpenAI**
- **Anthropic Claude**
- **Ollama** (local LLMs like LLaMA, Mistral, etc.)

---

## Key Features

- Multi-step task planning and execution  
- Natural language-based command composition  
- Flexible use of different LLM backends (OpenAI, Anthropic, Ollama)  
- Modular system to extend commands and tools easily  

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/CarlosBravoGarran/AI_Agent.git  #HTTPS
git clone git@github.com:CarlosBravoGarran/AI_Agent.git      #SSH
cd AI_Agent
```

### 2. Create and activate a virtual environment

```bash
python -m venv venv

# On Windows
venv\Scripts\activate

# On macOS / Linux
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure your API keys

Create a `.env` file in the root directory with your API keys:

```
OPENAI_API_KEY=your_openai_key
ANTHROPIC_API_KEY=your_anthropic_key
OLLAMA_URL=http://localhost:11434
```

⚠️ Note: `.env` is included in `.gitignore`, so it won’t be accidentally pushed to GitHub.

---

## Usage

Once everything is installed and configured, run the agent with:

```bash
python main.py
```

---

## Backend Comparison

| Backend   | Advantages                                         | Considerations                                 |
|-----------|----------------------------------------------------|------------------------------------------------|
| OpenAI    | High performance, official SDK, frequent updates   | Requires internet connection, may incur costs |
| Anthropic | Strong reasoning with Claude Sonnet                | Less widely adopted than OpenAI                |
| Ollama    | Private, no token cost, runs locally               | Requires installation and model download       |

---

## Requirements to Use Ollama

- Install [Ollama](https://ollama.com/)
- Download and run at least one model (e.g. LLaMA 3):

```bash
ollama run llama3
```

- Ensure the Ollama server is running at `http://localhost:11434` (default)

---

## Credits

- **Tech With Tim** – for the base tutorial  
- Adaptation with support for OpenAI, Anthropic Claude, and Ollama by [CarlosBravoGarran](https://github.com/CarlosBravoGarran)
