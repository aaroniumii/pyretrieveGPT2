# PyRetrieveGPT2
An interactive Python application that utilizes OpenAI and the Langchain library to retrieve and respond to user queries. It's primarily designed to fetch data from a dataset and present it in an appealing, user-friendly format. Unlike its predecessor which was a CLI (Command Line Interface) tool, this version allows users to interact through a web browser.

# Features
Interactive Command Line Interface (CLI): The application uses Typer to allow users to interact with the system via the command line in a conversational manner. 
Rich Text Output: The Rich library is used to format the console output, enabling the display of tables and colorized text. 
Information Retrieval: Leveraging the Langchain library, this application creates a semantic search index from a provided dataset (located in the "mydata" directory). It uses this index to retrieve relevant responses to user queries. 
Persistency: The application can optionally persist the semantic search index to disk, enabling faster startup times for subsequent runs.
Can be powered by GPT-4: Now OpenAI APIs are available, so can be used. 

# Usage
1. Locate the file(s) to read in the mydata folder. Files can be txt, pdf, docx, xls, html.
2. Set your OpenAI API Key in the credentials.py file.
3. Run the application with python pyretrieverGPT2.py .
4. The app will be served on http://0.0.0.0:5666/. Open the link in a browser so you can interact with it.
5. Simply type a query about your docs into the provided form and submit it.

To close, hit ctrl+c in the terminal.

# Dependencies
OpenAI: To generate semantic embeddings and responses. 
Langchain: For handling the creation and management of the semantic search index. 
Typer: To handle the interactive command line interface. Rich: To format console output.

Please refer to the requirements.txt file for a complete list of dependencies. Or you can install these packages with pip:

pip install flask langchain openai chroma vectorstore

Any improvement is welcome.
