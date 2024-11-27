# LLM-Security---Text-Prompt-Injection

## Overview
The **LLM Security** project is designed to protect Large Language Models (LLMs) from prompt injection attacks, which can lead to unintended, harmful, or malicious outputs. By using a combination of machine learning, heuristic rules, and vector-based similarity checks, this project ensures that LLMs produce safe and reliable responses even when exposed to potentially malicious inputs.

## Key Features
- **Logistic Regression Classification**: A trained model that identifies and classifies prompt injection attempts with high accuracy (0.965).
- **Heuristic Approach**: A rule-based method that analyzes inputs for suspicious patterns, keywords, and anomalies to detect harmful prompts.
- **Embedding-based Similarity Checks**: A vector database of embeddings is used to compare input prompts with known malicious patterns to detect potential threats.
- **Gradio Interface**: A user-friendly interface that allows real-time testing and deployment of the security measures.

## Technologies Used
- **Python**: The primary programming language used for implementing the logic, training models, and processing data.
- **Logistic Regression**: Used for classifying prompts as legitimate or injected based on trained features.
- **Heuristic Analysis**: A set of predefined rules that flag harmful inputs based on certain characteristics.
- **Vector Databases**: Embeddings of prompts are stored and compared to detect malicious inputs.
- **Gradio**: A Python library for building interactive interfaces for model testing and deployment.

## Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/llm-security.git
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the project:
    ```bash
    python app.py
    ```

   This will start a local server where you can interact with the LLM security interface via your web browser.

## Usage
Once the project is running, you can test the security of your LLM by entering prompts into the Gradio interface. The system will:
- Classify the prompt as either legitimate or suspicious.
- Check for potentially harmful keywords or patterns.
- Compare the prompt against a vector database of known prompt injections.

The final output will provide insights into whether the prompt is safe to process or needs to be flagged.

## Contributing
Contributions are welcome! Feel free to fork this repository, open issues, and submit pull requests. If you'd like to contribute to improving the security methods or adding new features, please ensure that your changes are well-documented and tested.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- **OpenAI**: For providing the inspiration and resources for working with large language models.
- **Scikit-learn**: For the logistic regression model and machine learning tools.
- **Gradio**: For making it easy to create interactive interfaces for machine learning models.
