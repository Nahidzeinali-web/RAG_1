# 🧠 RAG Implementation from Scratch with LLaMA2 Augmentation

This project demonstrates a **Retrieval-Augmented Generation (RAG)** pipeline using basic **cosine similarity** to find the most relevant document from a small corpus. It then augments the response using a **locally hosted LLaMA2 model** via [Ollama](https://ollama.com).

---

## 🚀 How It Works

1. **User query** is compared to a list of documents using bag-of-words + cosine similarity.
2. The **most similar document** is selected based on this score.
3. The selected document and query are passed to **LLaMA2** via a `POST` request to generate a concise recommendation.
4. The output is streamed and printed.

---

## 🧪 Example

**User input:**  
`i like to do yoga`

**Retrieved document:**  
`Take a yoga class and stretch your body and mind.`

**LLaMA2 Output:**  
> Try a yoga class to stretch and relax.

---

## 🛠️ Setup Instructions

### 1. Install Python packages

```bash
pip install requests
```

Or for full setup:

```bash
pip install -r requirements.txt
```

---

### 2. Install and run LLaMA2 with Ollama

Install Ollama from https://ollama.com, then run:

```bash
ollama pull llama2
ollama run llama2
```

---

### 3. Run the notebook

```bash
jupyter notebook RAG_implementation_from_scratch.ipynb
```

---

## 📁 Files

- `RAG_implementation_from_scratch.ipynb` — main notebook
- `requirements.txt` — Python dependencies
- `README.md` — (this file)

---

## 🙏 Acknowledgment

This implementation is inspired by tutorials from **Sunny Savita's YouTube channel**:

- [RAG Part 1](https://youtu.be/wTVTkOb3SZc?si=EWxVTxFSNqnoCK9N)
- [RAG Part 2](https://youtu.be/KyCtfQjkuR4?si=99FKEdNgDPiyxZ2W)
- [RAG Part 3](https://youtu.be/7k7tfxO4Zpw?si=XeMXH1UwToOIoClo)


## 📬 Contact

Feel free to reach out for suggestions, improvements, or collaboration ideas.
