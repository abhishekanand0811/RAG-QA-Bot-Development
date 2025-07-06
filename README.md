# Business RAG QA Bot

A Retrieval-Augmented Generation (RAG) chatbot for answering business-related questions using company documents.  
Combines OpenAI's GPT-4 and Pinecone vector search for accurate, context-aware answers.

---

## 🚀 Features

- Contextual Q&A using your own business documents
- Fast semantic search with Pinecone v3
- GPT-4 powered answer generation
- Source attribution for transparency
- Modular, extensible Python code

---

## 🛠️ Requirements

- Python 3.8+
- openai
- pinecone-client
- tiktoken
- python-dotenv
- numpy
- pandas

---

## 🔑 Setup

1. **Install dependencies:**
    ```
    pip install openai pinecone-client tiktoken python-dotenv numpy pandas
    ```

2. **Get API keys:**
    - [OpenAI API Key](https://platform.openai.com/account/api-keys)
    - [Pinecone API Key](https://www.pinecone.io/start/)

3. **Configure keys:**
    - Set your keys in the script or use a `.env` file.

---

## 📄 Usage

1. **Clone the repo:**
    ```
    git clone https://github.com/yourusername/business-rag-qa-bot.git
    cd business-rag-qa-bot
    ```

2. **Run the main script:**
    ```
    python business_rag_qa_bot.py
    ```

3. **Sample questions:**
    ```
    sample_questions = [
        "What is the work from home policy?",
        "What benefits are offered to employees?",
        "What are the security requirements?",
        # Add more questions as needed
    ]
    ```

---

## 📝 Example Output

Q: What is the work from home policy?
A: Employees can work from home up to 3 days per week with manager approval. Equipment and communication must be maintained.
Sources:

Company Policies - Remote Work (Score: 0.987)


---

## ⚙️ Customization

- **Add your own documents:**  
  Edit the `create_sample_business_data()` function.

- **Change chunk size or overlap:**  
  Modify `chunk_size` and `chunk_overlap` in the `BusinessRAGBot` class.

- **Switch models:**  
  Update `embedding_model` or `chat_model` as desired.

---

## 📚 References

- [OpenAI](https://openai.com/)
- [Pinecone](https://www.pinecone.io/)
- [tiktoken](https://github.com/openai/tiktoken)

---

## 📝 License

MIT License

---

*Contributions are welcome!*
