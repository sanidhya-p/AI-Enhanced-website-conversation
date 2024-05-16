This repository contains a web-based conversation chatbot built using Streamlit, OpenAI's UI, LangChain, Retrieval-Augmented Generation (RAG), and Chroma DB as the vector database. The chatbot is designed to engage users in meaningful conversations and provide accurate and contextually relevant responses.

Features
Web Interface: User-friendly interface built with Streamlit.
OpenAI UI: Utilizes OpenAI's advanced language model for generating responses.
LangChain: Manages and links various natural language processing (NLP) components.
Retrieval-Augmented Generation (RAG): Enhances response accuracy by retrieving relevant information from the database before generating a response.
Chroma DB: Efficiently stores and retrieves vectorized data to support the RAG mechanism.


Brief explanation of how RAG works

A RAG bot is short for Retrieval-Augmented Generation. This means that we are going to "augment" the knowledge of our LLM with new information that we are going to pass in our prompt. We first vectorize all the text that we want to use as "augmented knowledge" and then look through the vectorized text to find the most similar text to our prompt. We then pass this text to our LLM as a prefix.
![alt text](https://github.com/alejandro-ao/chat-with-websites/blob/master/docs/HTML-rag-diagram.jpg)
