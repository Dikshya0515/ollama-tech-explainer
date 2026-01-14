# AI Technical Question Answering Tool

A Python tool that uses Ollama's Llama 3.2 model to answer technical programming questions with detailed explanations.

## 🎯 Project Overview

This tool demonstrates the ability to integrate with AI APIs to create an interactive question-answering system. Users can input technical questions about code, programming concepts, or algorithms, and receive clear, detailed explanations.

## ✨ Features

- 🤖 Uses Llama 3.2 via Ollama (runs locally, completely free)
- ⚡ Streaming responses for real-time feedback
- 💬 Natural conversation-style explanations
- 🔒 Privacy-focused (everything runs on your machine)

## 🛠️ Prerequisites

Before running this project, you need:

1. **Python 3.8+** installed on your system
2. **Ollama** installed ([Download here](https://ollama.ai))
3. **JupyterLab** or Jupyter Notebook

## 📦 Installation

### Step 1: Install Ollama

1. Download Ollama from [https://ollama.ai](https://ollama.ai)
2. Install it on your system
3. Pull the Llama 3.2 model:
```bash
   ollama pull llama3.2
```

### Step 2: Install Python Dependencies
```bash
pip install ollama jupyter
```

### Step 3: Clone This Repository
```bash
git clone https://github.com/YOUR-USERNAME/ai-question-answering-tool.git
cd ai-question-answering-tool
```

## 🚀 Usage

1. Make sure Ollama is running on your system
2. Open JupyterLab:
```bash
   jupyter lab
```
3. Open the notebook file
4. Run all cells in order
5. Modify the `question` variable to ask your own questions!

### Example Questions
```python
# Example 1: Explain code
question = """
Please explain what this code does and why:
yield from {book.get("author") for book in books if book.get("author")}
"""

# Example 2: Concept explanation
question = """
What is the difference between a list and a tuple in Python?
"""

# Example 3: Algorithm question
question = """
Explain how binary search works and why it's efficient
"""
```

## 📁 Project Structure
```
ai-question-answering-tool/
│
├── notebook.ipynb          # Main Jupyter notebook
├── README.md              # This file
└── .gitignore            # Git ignore file
```

## 🔧 How It Works

1. **User Input**: You provide a technical question
2. **API Call**: The question is sent to Ollama's Llama 3.2 model
3. **Streaming Response**: The AI generates an answer in real-time
4. **Display**: The explanation is displayed word-by-word as it's generated

## 🎓 Learning Outcomes

This project demonstrates:
- Integration with local AI models using Ollama
- API communication and response handling
- Streaming data processing
- Building interactive educational tools

## ⚙️ Configuration

### Models Available

The project currently uses:
- `llama3.2` - Default model (lightweight and fast)

You can change the model by modifying:
```python
MODEL_LLAMA = 'llama3.2'
```

Other models you can try (after pulling them with `ollama pull MODEL_NAME`):
- `llama3.2:1b` - Smaller, faster
- `codellama` - Optimized for code
- `mistral` - Alternative model

## 🐛 Troubleshooting

### "Connection refused" error
- **Solution**: Make sure Ollama is running. Start it with `ollama serve` in terminal

### "Model not found" error
- **Solution**: Pull the model first with `ollama pull llama3.2`

### Slow responses
- **Solution**: Try a smaller model like `llama3.2:1b`

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

Your Name
- GitHub: [@yourusername](https://github.com/yourusername)

## 🙏 Acknowledgments

- [Ollama](https://ollama.ai) for providing the local AI infrastructure
- [Meta](https://www.meta.com) for the Llama model
- Course instructors for the project assignment

---

**Note**: This project was created as part of a course assignment to demonstrate familiarity with AI APIs and model integration.A