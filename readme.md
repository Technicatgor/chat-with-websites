# Chat with a Website from URL - LangChain Chatbot with Streamlit GUI

This repository is from the YouTube video tutorial available at <https://youtu.be/bupx08ZgSFg>. I have modified it to use local Ollama LLM. Please visit <https://www.youtube.com/@alejandro_ao> and subscribe to Alejandro_ao's channel. Thank you.

## Features

- **Website Interaction**: The chatbot uses the latest version of LangChain to interact with and extract information from various websites.
- **Large Language Model Integration**: Compatibility with models like GPT-4, Mistral, Llama2, and ollama. In this code I am using GPT-4, but you can change it to any other model.
- **Streamlit GUI**: A clean and intuitive user interface built with Streamlit, making it accessible for users with varying levels of technical expertise.
- **Python-based**: Entirely coded in Python.

## Brief explanation of how RAG works

A RAG bot is short for Retrieval-Augmented Generation. This means that we are going to "augment" the knowledge of our LLM with new information that we are going to pass in our prompt. We first vectorize all the text that we want to use as "augmented knowledge" and then look through the vectorized text to find the most similar text to our prompt. We then pass this text to our LLM as a prefix.

This is more clearly explained in the [Youtube video tutorial](https://youtu.be/bupx08ZgSFg), but here is a diagram that shows the process:

![RAG Diagram](docs/HTML-rag-diagram.jpg)

## Installation

Ensure that you have Python installed on your system. Afterward, clone this repository:

```bash
git clone [repository-link]
cd [repository-directory]
```

Install and run Ollama: <http://localhost:11434>
All of your local models are automatically served on <http://localhost:11434>.
Run "ollama run <name-of-model>" to start interacting via the command line directly.

Install the required packages:

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Usage

To run the Streamlit app:

```bash
streamlit run src/app.py
```

## Contributing

This repository is meant as supporting material for the [Youtube video tutorial](https://youtu.be/bupx08ZgSFg). Therefore, I am not accepting any pull requests unless they are for fixing bugs or typos.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

