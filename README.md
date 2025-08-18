# 💬 Chat App (FastAPI + JS)

A simple **chat application** built with FastAPI backend and responsive HTML/CSS/JS frontend.  
Supports **conversation IDs** so you can continue previous chats without a database.

---

## 🚀 Features
- FastAPI backend  
- Responsive UI (mobile + desktop)  
- Conversation ID for continuing chats  
- Gradient background & animations  

---

## 📂 Project Structure
- `app.py` → FastAPI backend  
- `index.html` → Frontend UI  
- `style.css` → Styling  
- `script.js` → Chat logic  
- `requirements.txt` → Dependencies  

---

## 🛠️ Setup
```bash
git clone https://github.com/anikchand461/chatbot.git
cd chatbot
cd backend
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
pip install -r requirements.txt
cd ..
```
create a .env file in the backend folder
```bash
GROQ_API_KEY=your_api_key_here
```
then...
```bash
uvicorn backend.app:app --reload
```
Then open the URL shown in your terminal (usually http://127.0.0.1:8000) in your browser.

## 📝 Usage
1.	Enter a Conversation ID.
2.	Start chatting with the assistant.
3.	Reuse the same ID to continue past chats.

## 🤖 LLM (Groq API)
- **Provider**: Groq  
- **Model**: llama-3.1-8b-instant  
- **Config**:  
  - temperature = 1  
  - max_tokens = 1024  
  - top_p = 1  
  - streaming enabled  

## ⚙️ Tech Stack
- **Backend**: FastAPI  
- **Frontend**: HTML, CSS, JavaScript  
- **LLM**: Groq API (LLaMA 3.1-8B Instant)  
- **Storage**: In-memory (conversation ID based)  