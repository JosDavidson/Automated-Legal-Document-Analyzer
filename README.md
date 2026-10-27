# Automated Legal Document Analyzer using GPT-4 ⚖️

An AI-powered legal document analysis and summarization system developed for **Experiment 5 (24CS2506 – Building Applications using GPT-4)**.

The system accepts legal contracts and agreements, extracts text and metadata, segments agreements into overlapping context chunks, formulates role-based constrained prompts, and produces structured legal analyses with risk compliance indicators.

---

## 🌟 Key Features

- **Zero Mobile Data / 100% Offline Execution**: Runs completely client-side in the browser or terminal with no mandatory network calls or external bloat.
- **Dual Engine Architecture**:
  - **Local Heuristic Legal Engine**: Instant, deterministic extraction with 0 mobile data usage.
  - **Live GPT-4 / Ollama API Connector**: Optional cloud or local LLM execution.
- **Contract Type Support**: Pre-configured templates and detection for:
  - Employment Agreements
  - Non-Disclosure Agreements (NDAs)
  - Master Services Agreements (MSAs)
  - Commercial Lease / Rental Agreements
- **Interactive Chunking Engine**: Visualizes document partitioning into sliding token windows with configurable chunk size and overlap buffers.
- **Structured Output Standard**:
  - Document Type & Identified Parties
  - Core Contractual Purpose
  - Duration & Term Milestones
  - Key Legal Obligations
  - Payment Terms & Remuneration Schedules
  - Termination Notice Conditions
  - Important Dates & Deadlines
  - Critical Clauses (Confidentiality, Liability, IP, Dispute Resolution) with risk assessment tags
  - Abstractive vs. Extractive summary comparison toggle

---

## 🏛️ System Architecture

```
[Legal Document (TXT/PDF/DOCX)]
              │
              ▼
    [Text Extraction Module]
              │
              ▼
   [Preprocessing & Cleaning]
              │
              ▼
 [Section / Chunk Identification]
              │
              ▼
   [Prompt Generation Module]
              │
              ▼
     [GPT-4 / AI Engine]
              │
              ▼
   [Structured Legal Analysis]
 (Parties, Clauses, Obligations, Dates, Summary)
```

---

## 🚀 Getting Started

### Method 1: Local Web Server (Node.js)
```bash
node server.js
```
Open **`http://localhost:3000`** in any web browser.

### Method 2: Direct Browser Launch
Simply open `index.html` in your browser. No server or internet connection required.

### Method 3: Python CLI
```bash
python legal_analyzer.py
```

---

## 📂 Project Structure

```
├── index.html            # Responsive front-end UI
├── styles.css            # Glassmorphism styling & animations (Dark/Light mode)
├── app.js                # Client application logic & intelligent legal parser
├── server.js             # Zero-dependency local Node.js server
├── legal_analyzer.py     # Python CLI & modular pipeline implementation
├── .gitignore            # Git exclusions
└── README.md             # Project documentation
```

---

## 📜 License
MIT License.
