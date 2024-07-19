

# NewsInsight: Intelligent News Analysis Tool 📈

NewsInsight is a Streamlit application designed to help users extract and analyze information from news articles. By providing URLs of news articles, the tool processes the content, creates embeddings, and allows users to query the information using OpenAI's language model.

## Features

- Extracts content from provided news article URLs.
- Splits the content into manageable chunks for processing.
- Creates embeddings using OpenAI embeddings.
- Stores the embeddings in a FAISS index.
- Allows users to query the stored information and retrieve answers along with their sources.

## Installation

To run this application, follow these steps:

### Prerequisites

- Python 3.7 or higher
- Git
- OpenAI API key

### Clone the Repository

```sh
git clone https://github.com/yourusername/NewsInsight.git
cd NewsInsight
```

### Create and Activate a Virtual Environment (optional but recommended)

```sh
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

### Install Dependencies

```sh
pip install -r requirements.txt
```

### Set Up Environment Variables

Create a `.env` file in the project directory and add your OpenAI API key:

```plaintext
OPENAI_API_KEY=your_openai_api_key
```

## Usage

### Running the Application

To start the Streamlit application, run:

```sh
streamlit run app.py
```

### Using the Application

1. **Enter URLs**: Use the sidebar to input up to three news article URLs.
2. **Process URLs**: Click the "Process URLs" button to load, split, and create embeddings for the articles.
3. **Ask Questions**: Once the processing is complete, you can enter your question in the main input field to retrieve answers and their sources.

### Example Workflow

1. Enter the URLs of the news articles you want to analyze.
2. Click the "Process URLs" button.
3. After processing, enter your question in the input field.
4. The application will display the answer and list the sources of information.

## Files and Structure

- `app.py`: Main application script.
- `requirements.txt`: List of dependencies.
- `.env`: Environment variables (not included in the repository).
- `faiss_store_openai.pkl`: Pickle file where the FAISS index is stored (generated after processing URLs).

