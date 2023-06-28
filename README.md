# 🤗💬 LLM Chat App
This project is a language model (LLM) powered chatbot, designed to comprehend and respond to questions based on an uploaded PDF file. It is built using [Streamlit](https://streamlit.io/), [LangChain](https://python.langchain.com/), and [HuggingFace](https://huggingface.co/) LLM models.

## About the App
The app uses the HuggingFace Instruct embeddings to understand the content of the PDF and answer the user's queries. The document is split into chunks and embeddings are created for each chunk. These embeddings are then stored and used to answer any queries related to the document. 

If you upload a PDF, the application will:
1. Extract the text from the PDF.
2. Split the text into chunks.
3. Compute embeddings for each chunk.
4. Store these embeddings for later use.
5. Accept user queries related to the PDF.
6. Search for the most relevant chunks to the query.
7. Use the LLM to generate a response to the query.

## Usage
To use the chatbot:
1. Clone this repository.
2. Replace "HUGGINGFACEHUB_API_TOKEN" with your HuggingFace API token in the `app.py` file.
3. Run the Streamlit app using the command `streamlit run app.py`.
4. Upload a PDF file using the file uploader in the Streamlit app.
5. Ask a question related to your PDF file in the provided text input field.
