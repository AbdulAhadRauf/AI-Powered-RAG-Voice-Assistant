# 🌾 AI-Powered Voice Assistant for Farmers

This project is a **RAG-powered voice assistant** designed to help farmers access information about government schemes like **PM-Kisan Yojna** and **Pradhan Mantri Matru Vandana Yojana (PMMVY)** in their native language. The system leverages **ASR, Translation, Vector Databases, and LLMs** to provide accurate responses to spoken queries.
<img width="1558" alt="download" src="https://github.com/user-attachments/assets/9680da21-97fd-49d0-9dcb-e65279dca74c" />


## 🚀 Features
- **Speech-to-Text (STT)**: Converts spoken queries into text using **AI4Bharat's IndicASR**.
- **Translation**: Converts Indic text to English (and vice versa) using **IndicTrans2**.
- **Retrieval-Augmented Generation (RAG)**: Fetches relevant scheme details from a **FAISS vector database**.
- **LLM Processing**: Uses **GPT-3.5-Turbo** to generate structured responses.
- **Text-to-Speech (TTS)**: Converts responses back to speech using **IndicTTS**.

## 📜 Workflow
1. **User Query**: The user asks a question in their native language.
2. **ASR Processing**: The audio query is transcribed into text using **IndicASR**.
3. **Translation**: The transcribed text is translated into English using **IndicTrans2**.
4. **Document Retrieval**: The query is matched against a **FAISS vector database** to fetch relevant scheme information.
5. **LLM Processing**: The retrieved document is processed using **GPT-3.5-Turbo**.
6. **Translation Back**: The response is translated back into the user’s original language.
7. **TTS Conversion**: The translated response is converted into speech using **IndicTTS** and played back to the user.
<img width="1390" alt="download (1)" src="https://github.com/user-attachments/assets/c37f1f45-d547-400c-8a0a-f3f7b55edd74" />


## 🛠️ Tech Stack
- **AI4Bharat Models**: IndicASR (ASR), IndicTrans2 (Translation), IndicTTS (TTS)
- **OpenAI GPT-3.5-Turbo**: LLM for generating responses
- **FAISS**: Vector search database for document retrieval
- **LangChain**: For integrating retrieval and LLM interaction
- **Python & FastAPI**: Backend processing

## ⚡ Setup Instructions
### Prerequisites
- Python 3.8+
- PIP & virtual environment (optional but recommended)

### Installation
```bash
# Clone the repository
git clone https://github.com/your-repo/ai-farmer-assistant.git
cd ai-farmer-assistant

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

# Install dependencies
pip install -r requirements.txt
```

### Running the Application
```bash
python main.py
```

## 📌 Future Enhancements
- Support for more Indian languages
- Mobile app integration
- Expansion to cover more government schemes

## 🤝 Contributing
Feel free to fork the repo, raise issues, and contribute! 

## 📜 License
MIT License

---

### 🔗 References
- [AI4Bharat Models](https://ai4bharat.org/)
- [OpenAI GPT-3.5-Turbo](https://openai.com/)
- [FAISS](https://github.com/facebookresearch/faiss)
- [LangChain](https://python.langchain.com/)
