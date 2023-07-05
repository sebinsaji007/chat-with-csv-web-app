

# chat with csv

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

> Now chat with your custom csv/excel files

This repository contains two Python files: `file1.py` and `file2.py`. These files are part of a project that enables users to interact with a CSV file using natural language queries. The project utilizes the OpenAI language model and the Streamlit framework.

## Prerequisites

To run the code in these files, you need to have the following prerequisites:

- Python 3.x
- `langchain` library (install using `pip install langchain`)
- `pandas` library (install using `pip install pandas`)
- `streamlit` library (install using `pip install streamlit`)

## Getting Started

Follow the steps below to get started with the project:

1. **Clone** this repository to your local machine.
2. Install the required libraries as mentioned in the prerequisites.
3. Set up the API key for the OpenAI language model. You can obtain the API key from [OpenAI](https://openai.com/).
4. Create a **virtual environment** (recommended) and activate it.
5. Run `file2.py` using the command `streamlit run file2.py`.
6. The Streamlit app will open in your browser.
7. Upload a CSV file by clicking the "Upload a CSV file" button.
8. Enter your query in the text area provided.
9. Click the "Submit Query" button to see the results.

## File Descriptions

### `file1.py`

This file contains the following functions:

- `create_agent(filename: str)`: Creates an agent using the OpenAI language model and a CSV file specified by the `filename` parameter.
- `query_agent(agent, query)`: Queries the agent with a natural language query and returns the response.

### `file2.py`

This file contains a Streamlit app that allows users to interact with a CSV file using natural language queries. It includes the following functions:

- `decode_response(response: str) -> dict`: Decodes the response string from the agent into a dictionary.
- `write_response(response_dict: dict)`: Writes the response from the agent to the Streamlit app.
- Streamlit app components:
  - File uploader: Allows users to upload a CSV file.
  - Text area: Users can enter their queries.
  - Submit button: Triggers the query and displays the response.

## Usage

To use the project, follow these steps:

1. Ensure you have met the prerequisites mentioned earlier.
2. Provide the API key for the OpenAI language model in `file1.py`.
3. Run `file2.py` using the command `streamlit run file2.py`.
4. Interact with the Streamlit app by uploading a CSV file and entering queries.

Feel free to modify the code and adapt it to your specific needs.

## Contributing

Contributions are welcome! Please feel free to submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
