
# MultiPDFChatHub App

## Introduction
------------
The MultiPDFChatHub app is a Python application that lets you communicate with multiple PDF documents. You can ask questions about the PDFs in natural language, and the application will respond appropriately based on the content of the documents. This app uses a language model to provide accurate responses to your questions. Please keep in mind that the app will only answer questions about the PDFs you've loaded.


## How It Works
------------

![MultiPDFChatHub app diagram](https://github.com/Kamal934/Chat-wth-Multiple-PDF/assets/110932441/1779ca38-2a1b-40a1-aa42-fbd761e4ae08)


The appliction following these steps to provide the respond your questions:

1. Multiple Pdf Loading: The app reads the multiple Pdf and extract their content.

2. Text Chunking: The extracted text is dividing into the number of smaller chunks that can be  processed effiectively.

3.  Language Model: The application utilizes a language model to generate vector representations (embeddings) of the text chunks.

4. Similarity Matching: When you ask a question, the app compares it with the text chunks and identifies the most semantically similar ones.

5. Response Generation: The selected chunks are passed to the language model, which generates a response based on the relevant content of the PDFs.

## Dependencies and Installation
----------------------------
To install the MultiPDFChatHub App, please follow these steps:

1. Clone the repository to your local machine.

2. Install the required dependencies by running the following command:
   ```
   pip install -r requirements.txt
   ```

3. Obtain an API key from OpenAI and add it to the .env file in the project directory. (in this repository .env file is the name of .env.apikey when you are cloning  the repository change file name into .env )
```commandline
OPENAI_API_KEY=your_secrit_api_key
```

## Usage
-----
To use the MultiPDFChatHub App, follow these steps:

1. Ensure that you have installed the required dependencies and added the OpenAI API key to the `.env` file.

2. Run the `main.py` file using the Streamlit CLI. Execute the following command:
   ```
   streamlit run app.py
   ```

3. The application will launch in your default web browser, displaying the user interface.

4. Load multiple PDF documents into the app by following the provided instructions.

5. Ask questions in natural language about the loaded PDFs using the chat interface.


## License
-------
The MultiPDFChatHub App is released under the [MIT License](https://opensource.org/licenses/MIT).

