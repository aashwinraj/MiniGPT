# 🧠 MiniGPT — Lightweight Text Generation Model

MiniGPT is a minimal yet functional GPT-style text generation project built from scratch using **PyTorch** and deployed via a **FastAPI** inference API.

It demonstrates a full mini-LLM lifecycle — **training**, **saving checkpoints**, and **serving text generation via an HTTP endpoint**.

---

## 🚀 Features

- 🧩 **Custom GPT-style architecture** implemented in PyTorch  
- 🏋️‍♂️ **Trained on tokenized text data** (Byte Pair Encoding vocabulary)  
- 💾 **Checkpoint saving & loading** for model reuse  
- ⚙️ **FastAPI inference server** exposing a `/generate` endpoint  
- 🔥 **GPU acceleration (if available)** using `torch.cuda`  
- 📦 **Clean project structure** with tokenizer, model, and inference neatly organized  

---

uvicorn app:app --reload --port 8080
curl -X POST "http://127.0.0.1:8080/generate" \
  -H "Content-Type: application/json" \
  -d '{
    "prompt": "I am a boy from",
    "max_new_tokens": 150
  }'
  <img width="1419" height="867" alt="Screenshot 2025-11-04 161758" src="https://github.com/user-attachments/assets/aa8a6b46-ca5a-4873-8300-f1344e89ff0a" />


