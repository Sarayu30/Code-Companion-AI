 

# Code Companion AI 🧠

**DeepSeek: Your AI Pair Programmer with Debugging Superpowers**

This is a Streamlit-based app that integrates **Ollama** and **LangChain** to create a chatbot that assists you with coding tasks, debugging, code documentation, and solution design.

## Features

- **🐍 Python Expert**: Ask anything about Python, and the AI will help you.
- **🐞 Debugging Assistant**: Get help debugging your code with strategic print statements and concise solutions.
- **📝 Code Documentation**: Generate documentation for your code automatically.
- **💡 Solution Design**: Receive suggestions and improvements for your code structure.

## Requirements

- **Ollama**: The chatbot engine used to provide AI solutions. You can install it from [Ollama](https://ollama.ai/).
- **LangChain**: A framework for building applications with LLMs (Language Models). [LangChain documentation](https://python.langchain.com/).

### Installation

1. Install the required libraries by running:

    ```bash
    pip install streamlit langchain langchain-ollama
    ```

2. Ensure that **Ollama** is installed and running locally on your system. Start Ollama by following the instructions from [Ollama](https://ollama.ai/).

3. Start the Streamlit app:

    ```bash
    streamlit run app.py
    ```

4. The app will be available in your browser at `http://localhost:8501/`.

---

## How to Use

- **Choose Model**: Select your preferred model (e.g., `deepseek-r1:1.5b` or `deepseek-r1:3b`) from the sidebar configuration. 
- **Ask Coding Questions**: Type your coding-related queries in the chat input box. For example:
  - "How do I debug this code?"
  - "Can you help me with a Python function?"
  - "What's wrong with my code?"
- **View Responses**: Once your query is processed, the AI will provide concise, accurate, and debug-ready solutions.
- **Debugging**: The AI will assist with debugging by strategically adding print statements and pinpointing issues.

---

## Customization

- **Temperature**: The temperature parameter (`temperature=0.3`) controls the randomness of the AI's responses. You can modify this in the `llm_engine` initialization.

- **Model Selection**: The available models are `deepseek-r1:1.5b` and `deepseek-r1:3b`. You can customize the `selected_model` parameter in the app.

---

## Technical Details

- **LangChain Integration**: The app uses LangChain's `ChatOllama` module to communicate with the AI model, ensuring smooth integration with Ollama.
- **Custom Prompt**: A custom system prompt is defined to ensure that the AI behaves as an expert coding assistant.
- **State Management**: The session state keeps track of the conversation history, so the chatbot can remember previous messages and maintain context.

---
 
## Acknowledgments

- **Ollama**: For providing the powerful language model for this application.
- **LangChain**: For simplifying the process of integrating language models into applications.
 
