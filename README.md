# *MultiPDF Chat App*: An Advanced Python-Based Query Interface

## Project Overview:

The MultiPDF Chat App is an innovative Python-based application designed to interactively communicate with multiple PDF documents simultaneously. Leveraging the power of natural language processing, users can pose questions in conversational language and receive precise answers extracted directly from the content within the PDFs. This sophisticated application employs a cutting-edge language model to ensure the accuracy and relevance of responses to user inquiries. It is important to note that the application's scope is confined to the PDF documents currently loaded, and as such, it will only address queries that pertain to the information contained therein.

# A Step-by-Step Overview of the Query Response Mechanism


![MultiPDF Chat App Diagram](./png/PDF-LangChain.jpg)


1. **PDF Loading:** The app reads multiple PDF documents and extracts their text content.

2. **Text Chunking:** The extracted text is divided into smaller chunks that can be processed effectively.

3. **Language Model:** Leveraging an open-source Embedding model from HuggingFace, the app creates vector representations of these chunks.

4. **Similarity Matching:** When you ask a question, the app compares it with the text chunks and identifies the most semantically similar ones.

5. **Response Generation:** These chunks are then passed to the OpenAI LLM, which crafts a response that’s informed by the relevant PDF content.


# Dependencies and Installation:

To install the MultiPDF Chat App, please follow these steps:

1. Clone the repository to your local machine.

2. Install the required dependencies by running the following command:
   ```
   pip install -r requirements.txt
   ```

3. Obtain an API key from OpenAI and add it to the `.env` file in the project directory.
    ```commandline
    OPENAI_API_KEY=your_secrit_api_key
    ```