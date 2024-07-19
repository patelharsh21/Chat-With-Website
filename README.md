
NewsInsight: Intelligent News Analysis Tool📈
NewsInsight is a Streamlit application designed to help users extract and analyze information from news articles. By providing URLs of news articles, the tool processes the content, creates embeddings, and allows users to query the information using OpenAI's language model.

Features
Extracts content from provided news article URLs.
Splits the content into manageable chunks for processing.
Creates embeddings using OpenAI embeddings.
Stores the embeddings in a FAISS index.
Allows users to query the stored information and retrieve answers along with their sources.
Installation
To run this application, follow these steps:

Prerequisites
Python 3.7 or higher
Git
OpenAI API key
Clone the Repository
sh
Copy code
git clone https://github.com/yourusername/RockyBot.git
cd NewsInsight: Intelligent News Analysis Tool
Create and Activate a Virtual Environment (optional but recommended)
sh
Copy code
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
Install Dependencies
sh
Copy code
pip install -r requirements.txt
Set Up Environment Variables
Create a .env file in the project directory and add your OpenAI API key:

plaintext
Copy code
OPENAI_API_KEY=your_openai_api_key
Usage
Running the Application
To start the Streamlit application, run:

sh
Copy code
streamlit run app.py
Using the Application
Enter URLs: Use the sidebar to input up to three news article URLs.
Process URLs: Click the "Process URLs" button to load, split, and create embeddings for the articles.
Ask Questions: Once the processing is complete, you can enter your question in the main input field to retrieve answers and their sources.
Example Workflow
Enter the URLs of the news articles you want to analyze.
Click the "Process URLs" button.
After processing, enter your question in the input field.
The application will display the answer and list the sources of information.
Files and Structure
app.py: Main application script.
requirements.txt: List of dependencies.
.env: Environment variables (not included in the repository).
faiss_store_openai.pkl: Pickle file where the FAISS index is stored (generated after processing URLs).



