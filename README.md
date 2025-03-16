# Chatbot Project

## Overview
This project is a simple AI-powered chatbot built using Python and Streamlit. It leverages Natural Language Processing (NLP) techniques to understand and respond to user queries. The chatbot is designed to assist users with predefined intents and responses stored in a JSON file.

## Features
- User-friendly interface with Streamlit
- NLP-based response generation using `nltk` and `scikit-learn`
- Intent recognition via TF-IDF Vectorization
- Customizable responses stored in `intents.json`
- Easy to modify and expand

## Installation
To set up the chatbot on your local machine, follow these steps:

### Prerequisites
Ensure you have **Python 3.7+** installed.

### Install Required Packages
Run the following command to install dependencies:
```sh
pip install -r requirements.txt
```
If `requirements.txt` is not available, install packages manually:
```sh
pip install streamlit nltk scikit-learn pandas
```

## Running the Chatbot
Start the chatbot using the following command:
```sh
streamlit run chatbot.py
```
This will open the chatbot interface in your default web browser.

To run Streamlit, navigate to the folder where your chatbot script is stored and execute the above command in **Command Prompt (Windows)**, **VS Code Terminal**, or **Mac/Linux Terminal**. Ensuring that you are in the correct directory is essential before running the command.

## File Structure
```
chatbot/
│── chatbot.py          # Main script to run the chatbot
│── intents.json        # JSON file containing predefined intents and responses
│── requirements.txt    # List of dependencies
│── README.md           # Project documentation
```

## Customization
You can modify `intents.json` to add new responses:
```json
{
  "intents": [
    {
      "tag": "greeting",
      "patterns": ["Hello", "Hi", "Hey"],
      "responses": ["Hi there!", "Hello!", "Hey!"]
    }
  ]
}
```

## Troubleshooting
### `ModuleNotFoundError`
If you encounter missing module errors, ensure all dependencies are installed:
```sh
pip install -r requirements.txt
```
### JSON Errors
Ensure `intents.json` is properly formatted by validating it at [jsonlint.com](https://jsonlint.com/).

## Contributing
Feel free to enhance this chatbot by improving NLP processing or adding new features. Contributions are welcome!

## License
This project is licensed under the MIT License.





      
