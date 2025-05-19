# med-ally-ai

# 🩺 MED-ALLY: Offline AI Medical Copilot

**MED-ALLY** is a privacy-first, fully offline AI assistant designed to help doctors, field medics, and healthcare workers analyze medical cases — even in low-connectivity environments.

## 🚀 What It Does

- Upload a PDF medical report or enter symptoms manually
- Extracts vitals, symptoms, medications using NLP + NER
- Suggests likely diagnoses using a local LLM
- Checks for drug interactions using a local database
- Outputs a structured summary or triage recommendation

## 🌐 Why It Matters

Medical decision support is critical — but expensive cloud tools, API limits, or connectivity issues limit adoption. MED-ALLY is designed to work **offline**, **freely**, and **privately** for clinics, NGOs, and field hospitals.

## 🧠 Stack

| Component | Tool |
|----------|------|
| UI | Streamlit |
| LLM | Mistral 7B / Mixtral (via Ollama or HuggingFace Transformers) |
| NER | spaCy + Transformers |
| PDF Parsing | pdfplumber |
| Memory | ChromaDB |
| Drug DB | Local JSON lookup |
| TTS (optional) | Coqui TTS |

## 🗂 Folder Structure

```bash
app/               # Application logic (input, core engine, output)
data/              # Sample PDFs, drug database
models/            # LLM-related embeddings / weights
utils/             # NLP tools, vector search
docs/              # Architecture diagram, usage guide
