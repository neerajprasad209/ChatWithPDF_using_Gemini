# *MultiPDF Chat App*: An Advanced Python-Based Query Interface

## Project Overview:

The MultiPDF Chat App is an innovative Python-based application designed to interactively communicate with multiple PDF documents simultaneously. Leveraging the power of natural language processing, users can pose questions in conversational language and receive precise answers extracted directly from the content within the PDFs. This sophisticated application employs a cutting-edge language model to ensure the accuracy and relevance of responses to user inquiries. It is important to note that the application's scope is confined to the PDF documents currently loaded, and as such, it will only address queries that pertain to the information contained therein.

# A Step-by-Step Overview of the Query Response Mechanism


![MultiPDF Chat App Diagram](./png/PDF-LangChain.jpg)


1. **Document Ingestion**: The application commences by loading multiple PDF documents, meticulously extracting the textual data contained within each file.

2. **Data Segmentation**: Subsequent to extraction, the text is systematically segmented into manageable portions, optimizing the processing workflow.

3. **Cognitive Processing**: Utilizing an advanced language model, the app constructs vector representations, known as embeddings, for each segmented text portion, facilitating nuanced understanding.

4. **Semantic Analysis**: Upon receiving a user query, the application performs a semantic comparison between the query and the text embeddings, pinpointing the segments with the highest semantic correlation.

5. **Intelligent Synthesis**: The final step involves the language model synthesizing a coherent and contextually relevant response, drawing from the content of the identified text segments.

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