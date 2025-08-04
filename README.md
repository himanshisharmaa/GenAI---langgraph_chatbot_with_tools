LangGraph Chatbot with Third-Party Tools

This repository contains a LangGraph-powered chatbot that intelligently uses external tools to answer user questions. The chatbot is designed to first attempt to answer queries using its own knowledge, and if it cannot, it will then consult specialized third-party tools such as Arxiv and Wikipedia to retrieve information.

Features

* Intelligent Question Answering: The chatbot determines when to use external tools for better answers.
* Tool Integration: Seamlessly uses Arxiv for scientific papers and Wikipedia for general knowledge.
* LangGraph Framework: Built using LangGraph for a robust and modular agentic workflow.
* Groq Powered: Leverages the Groq API for fast and efficient language model inference with the Gemma2-9b-It model.

Getting Started

To run this chatbot, follow these steps:

Prerequisites

* Python 3.8+
* pip

Installation

1.  Clone this repository or download the langgraph_chatbot_with_tools.ipynb file.

2.  Install the required Python packages:
    pip install langgraph langsmith langchain langchain_groq langchain_community arxiv wikipedia

API Key Setup

This project uses the Groq API. You will need a Groq API key.

1.  Obtain your Groq API Key from the Groq console.
2.  Store your API key securely. If running in Google Colab, you can use `userdata.get("GROQ_API_KEY")`. Otherwise, it's recommended to use environment variables (e.g., in a .env file) to load your API key.

Running the Notebook

1.  Open the langgraph_chatbot_with_tools.ipynb file in a Jupyter environment (like Jupyter Notebook, JupyterLab, or Google Colab).
2.  Execute all the cells in the notebook sequentially.
3.  Ensure your Groq API key is correctly configured in the `groq_api_key=userdata.get("GROQ_API_KEY")` line or equivalent.
4.  You can then interact with the chatbot by modifying the `user_input` variable and re-running the relevant cells.

Example Usage

The notebook includes example prompts demonstrating how the chatbot interacts and utilizes its tools.

Configuration

* ArxivAPIWrapper: Configured to retrieve 1 result with a maximum content length of 300 characters.
* WikipediaAPIWrapper: Configured to retrieve 1 result with a maximum content length of 300 characters.
* LLM Model: The default model used is Gemma2-9b-It from Groq.

Contributing

Feel free to open issues or submit pull requests if you have suggestions for improvements or new features.

License

This project is open source. (Consider adding a LICENSE file, e.g., MIT License)

Acknowledgements

* LangChain
* LangGraph
* Groq
* Arxiv
* Wikipedia
```
