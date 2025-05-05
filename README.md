# 🤖 Income Tax Chatbot Assistant 💰

**AI-Powered Tax Consultation System**  
*Streamlit-based chatbot providing instant answers about Indian income tax slabs and regimes using Gemini AI + FAISS semantic search*


## 📌 Overview
An intelligent chatbot that helps users understand:
- New vs Old Tax Regimes 📊
- Income Tax Slabs 📈
- Budget Changes 💼
- Tax Deductions & Exemptions 🧾
- Surcharge Rates 📋
- Section 87A Rebates 🛡️

Combines semantic search with LLM-powered explanations for accurate, user-friendly tax guidance.

## ✨ Key Features
- **📚 Dual Knowledge Base**: Pre-defined Q&A + Gemini-generated explanations
- **🔍 Context-Aware Search**: FAISS vector similarity for precise answer retrieval
- **💬 Natural Interactions**: Human-like conversational responses
- **🎯 Error Handling**: Graceful fallback for out-of-scope questions
- 📱 Mobile-Responsive UI with Tax-Themed Design
- 🔄 Dynamic Data Loading (Easy CSV updates)

## 🛠️ Tech Stack
| Component | Technology | Purpose |
|-----------|------------|---------|
| Frontend | `Streamlit` | Web Interface |
| AI Engine | `Google Gemini-1.5-Flash` | Response Generation |
| NLP | `sentence-transformers/all-MiniLM-L6-v2` | Text Embeddings |
| Search | `FAISS` | Semantic Matching |
| Data | `Pandas` | CSV Processing |
| Backend | `Python 3.10` | Core Logic |

## 🚀 Installation
1. **Clone Repository**
   ```bash
   git clone https://github.com/yourusername/tax-chatbot.git
   cd tax-chatbot

2. **Set Up Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate  # Windows
   pip install -r requirements.txt

3. **Get Gemini API Key**
   - Visit [Google AI Studio](https://makersuite.google.com/app).
   - Create a new **API key**.
   - Replace the placeholder in `app.py` with your actual API key:
     ```python
     genai.configure(api_key="YOUR_ACTUAL_API_KEY_HERE")

4. **Run Application**
   ```bash
   streamlit run app.py

## 💻 Usage

Access the chatbot at [http://localhost:8501](http://localhost:8501)

Ask questions like:

- "Compare new vs old tax regimes?"
- "What's the surcharge rate above 2 crore?"
- "Explain Section 87A rebate with example"

### ✨ Features

- ✅ Context-aware follow-up questions  
- 🚫 Automatic out-of-scope detection  
- 📚 Multi-layered explanations for complex queries


## 📂 Data Management

To update or customize tax-related information:

**🔧 Modify in Code**
- Update the `load_data()` function in `app.py` to reflect new Q&A pairs.
- Maintain the following format:
  ```python
  data = {
  "question": ["..."],
  "answer": ["..."]
  }

## 🎨 UI Customization

You can customize the chatbot's appearance by modifying the CSS inside the `st.markdown` block in `app.py`.

- Example
  ```css
  .chat-font {
  font-family: 'Your Font';
  color: #your-color;
  }
  .user-msg {
  border-color: #your-color;
  }


## 🤝 Contributing

We welcome contributions! To get started:

1. **Fork** the repository
   
2. **Create your feature branch**  
   ```bash
   git checkout -b feature/amazing-feature

3. **Commit your changes**  
   ```bash
   git commit -m 'Add amazing feature'

4. **Push to the branch**  
   ```bash
   git push origin feature/amazing-feature

5. **Open a Pull Request** on GitHub

## 📜 License

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This project is distributed under the **MIT License**.  
For more details, please refer to the [LICENSE](LICENSE) file.

## 📞 Contact

**Project Maintainer**  
[Dutta Krishna Madhumita]  
📧 [krishnamadhumitadutta@gmail.com](mailto:krishnamadhumitadutta@gmail.com)
