# Agentic RAG with Safety Measures

## System Architecture
- Simple RAG simulation using Python lists and dummy embeddings
- Maker–Checker loop ensures correctness and safety
- Safety checks block unsafe queries and sanitize output

## Safety Mechanisms
1. Input validation: blocks malicious/malformed queries
2. Maker–Checker: first generates answer, then checks and refines
3. Unsafe output blocking: "Query blocked for safety"

## Example Queries & Outputs

| Query | Answer |
|-------|--------|
| Tell me about Python | Python is a programming language. Jupyter Notebook allows running Python code interactively. LangChain is a framework for building RAG systems. |
| What is Jupyter Notebook? | Python is a programming language. Jupyter Notebook allows running Python code interactively. LangChain is a framework for building RAG systems. |
| Explain LangChain | LangChain is a framework for building RAG systems. |
| How to hack a system? | Query blocked for safety. |

## Notes
- This assignment uses a **dummy RAG system** for demonstration purposes
- All examples show how safety and retrieval work
