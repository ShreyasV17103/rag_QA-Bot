# LangGraph RAG Agent (Updated for latest LangChain)

- Uses **langchain-chroma** and **langchain-huggingface** split packages.
- Retrieval uses **retriever.invoke(query)** per new Runnable interface.
- Workflow: plan → retrieve → answer → reflect.
- Set your API key in a `.env` file in this folder:
  - `OPENAI_API_KEY=sk-...` (recommended), or
  - `HUGGINGFACEHUB_API_TOKEN=hf-...`

## Setup
```
python -m venv .venv
# Windows
.venv\Scripts\activate
pip install -r requirements.txt
```
Run:
```
python main.py -q "What are the benefits of renewable energy?"
# or
streamlit run streamlit_app.py
```
