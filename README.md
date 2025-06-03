# Extracting-Information-from-Legal-Documents-Using-RAG-
This project leverages **Retrieval-Augmented Generation (RAG)** to build an intelligent Question Answering (QA) system over complex legal documents. The solution uses advanced language models and vector similarity search to accurately retrieve and respond to legal queries, helping improve legal research efficiency and compliance analysis.

---

## 🎯 Business Objective

To automate and streamline the process of querying legal documents—such as contracts, privacy policies, and NDAs—by providing relevant, contextual, and accurate answers to user queries using a Retrieval-Augmented Generation framework.

This is aimed at assisting:
- Legal professionals during contract review and clause verification  
- Compliance teams in quickly retrieving obligations and policy terms  
- Organizations in improving access to critical legal information without manual reading

---

## 📌 Scope of the Project

- Focused on building a **domain-specific QA system** that can:
  - Understand legal queries in natural language  
  - Retrieve relevant context from large legal documents  
  - Generate accurate and trustworthy answers  
- Evaluation of the generated responses using both **linguistic** and **semantic** metrics  
- Ensuring that answers are not only correct but derived from the proper source context

---

## 🛠️ Methodologies Followed

### 1. **Document Parsing & Preprocessing**
- Load legal documents from a structured folder hierarchy  
- Clean and segment documents into manageable text chunks (~512 tokens)

### 2. **Embedding & Vector Indexing**
- Use OpenAI’s Embedding model to convert text chunks into vector representations  
- Store embeddings in a FAISS vector database for fast semantic retrieval

### 3. **Query Handling with RAG Pipeline**
- Accept legal queries and retrieve the top-k most relevant chunks  
- Use `RetrievalQA` with a language model to generate contextual answers

### 4. **Evaluation & Validation**
- Compare generated answers against ground truth using:
  - **ROUGE-L** for text overlap
  - **BLEU** for linguistic accuracy
  - **RAGAS metrics** for:
    - Faithfulness
    - Answer Relevancy
    - Context Recall

---

## 📈 Evaluation Summary (Sample Output)

| Metric              | Score     |
|---------------------|-----------|
| ROUGE-L             | 0.84      |
| BLEU                | 67.48     |
| Answer Relevancy    | 0.952     |
| Faithfulness        | 0.803     |
| Context Recall      | 0.945     |

> The high answer relevancy and context recall reflect the model’s reliability in drawing accurate responses directly from relevant legal text segments.

---

## ✅ Key Insights

- RAG-based systems are highly effective for **knowledge-intensive domains** like law  
- Embedding-driven retrieval ensures the generated content is **fact-grounded and precise**  
- Metrics show **consistency in aligning answers with trusted legal sources**, which is essential for use in regulated environments

---

## 🚀 Potential Extensions

- Add support for summarization and clause tagging  
- Build a chatbot-style frontend for real-time interaction  
- Train with additional legal corpora to enhance domain adaptation  
- Extend support for multilingual legal queries

---

## 👨‍💻 Author

**Akshat Singh Patel**  
_Data Science | NLP 
