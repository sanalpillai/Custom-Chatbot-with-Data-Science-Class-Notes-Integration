# Custom Chatbot with Data Science Class Notes Integration

This repository hosts a Python project that integrates class notes into a custom chatbot, leveraging OpenAI's GPT models for enhancing educational interactions. The chatbot first attempts to find answers within the provided class notes. If it doesn't find a relevant answer, it then uses OpenAI's GPT-3.5-turbo model to generate responses.

## Features

- **Text Extraction from PDF**: Employs PyMuPDF for extracting text from class notes stored in PDF files.
- **OpenAI API Integration**: Uses OpenAI's API to fetch intelligent responses for queries not covered by class notes.
- **Priority on Educational Content**: Ensures responses are primarily based on the educational content from class notes.

## Setup

### Prerequisites

- Python 3.x installed
- An active OpenAI API key

### Installation

Install the necessary dependencies with pip:

```bash
pip install openai==0.28 PyMuPDF
```

### Configuration
Securely set your OpenAI API key as an environment variable:

```python
import os
os.environ["OPENAI_API_KEY"] = "your_api_key_here"
```

Replace _"your_api_key_here"_ with your actual OpenAI API key.

### Usage
Ensure the class notes PDF is in the same directory as the script. Run the script, and input your queries when prompted. Type quit to exit the conversation.

```bash
python your_script_name.py
```

### Project Structure
- **extract_text_from_pdf:** Extracts text from a specified PDF file of class notes.
- **chatbot:** Initiates the chatbot, accepting user queries and responding with relevant information.

### Contributing
Contributions, issues, and feature requests are welcome. Feel free to check issues page for more information.

### License
This project is licensed under the MIT License - see the LICENSE file for details.
