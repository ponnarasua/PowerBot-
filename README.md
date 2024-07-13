Certainly! Here's a README file for your Streamlit MineBot project:

---

# PowerBot
chatbot for power substations
## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/minebot.git
    cd minebot
    ```

2. **Create a virtual environment and activate it**:
    ```bash
    python -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. **Install the required packages**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Set up environment variables**:
    Create a `.env` file in the root directory and add your OpenAI and SerpAPI keys:
    ```
    OPENAI_API_KEY=your_openai_api_key
    SERPAPI_API_KEY=your_serpapi_api_key
    ```

5. **Download the embedding model and index**:
    - Ensure the embedding model `BAAI/bge-large-en-v1.5` is available in the `model_cache` folder.
    - Ensure the FAISS index `clean_total_index_bge_large` is available in the root directory.

## Usage

1. **Run the Streamlit app**:
    ```bash
    streamlit run app.py
    ```

2. **Activate the system**:
    - Go to the sidebar and click on "Activate" to load the models and tools.

3. **Start chatting**:
    - Use the chat input at the bottom of the page to ask questions related to mining regulations, and the bot will respond accordingly.

## Project Structure

```
minebot/
├── .env.example          # Example environment file
├── app.py                # Main application file
├── requirements.txt      # List of Python dependencies
├── model_cache/          # Directory for embedding model cache
└── clean_total_index_bge_large  # FAISS index file
```

## Customization

- **CSS and HTML Templates**:
  - Customize the look and feel of the chat interface by modifying the `CSS`, `bot_template`, and `user_template` variables in `app.py`.

- **Tools and Memory**:
  - Add or modify tools in the `get_tools` function.
  - Change memory settings in the `get_memory` function.

## Contributing

1. **Fork the repository**.
2. **Create a new branch**:
    ```bash
    git checkout -b feature/your-feature-name
    ```
3. **Make your changes**.
4. **Commit your changes**:
    ```bash
    git commit -m "Add some feature"
    ```
5. **Push to the branch**:
    ```bash
    git push origin feature/your-feature-name
    ```
6. **Open a pull request**.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [Streamlit](https://streamlit.io/)
- [Langchain](https://langchain.com/)
- [OpenAI](https://openai.com/)
- [HuggingFace](https://huggingface.co/)

---

Feel free to customize the README further to fit your specific needs.
