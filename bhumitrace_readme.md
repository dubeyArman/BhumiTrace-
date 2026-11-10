# BhumiTrace : 

**Untangling legacy land records to unlock financial security.**

BhumiTrace is an AI-powered digitization platform designed to process old, handwritten property documents, extract key ownership data, and generate a bank-ready visual "Ownership Timeline."

##  The Problem

For many rural families, land records consist of a confusing trail of regional language documents (like Khasra or Khatauni). This makes proving a clear title for a bank loan, inheritance, or sale extremely difficult. The wealth exists, but it is locked behind unclear, messy paperwork.

## 💡 Our Solution

BhumiTrace solves this through a straightforward, three-step digital workflow:

1. **Smart Digitization:** Users upload photos of physical land documents.

2. **Lineage Mapping:** The platform extracts the data and builds a chronological "Ownership Tree."

3. **Discrepancy Engine:** The system cross-references the data to flag missing mutations, spelling mismatches, or unreleased bank liens, acting as a "Land Health Card."

## 🛠️ Proposed Tech Stack

### Frontend

* **Framework:** React.js / Vite

* **Styling:** Tailwind CSS (for an accessible, clean UI)

* **Visualizations:** React Flow (for generating the Ownership Tree timeline)

### Backend & AI

* **Framework:** Python / FastAPI (for rapid, lightweight endpoint generation)

* **OCR / Data Extraction:** Tesseract OCR / Google Cloud Vision API

* **Data Parsing:** Basic LLM prompt engineering to structure the extracted regional text into JSON format.

* **Database:** PostgreSQL (for relational data linking owners to land parcels)

## ⚙️ Planned System Architecture

1. **Client Layer:** React web app captures the document image and sends it via REST API.

2. **Processing Layer:** FastAPI receives the image, routes it to the OCR engine, and parses the raw text into structured data (Owner Name, Survey Number, Date, Transaction Type).

3. **Logic Layer:** The Discrepancy Engine checks the extracted JSON against standard historical flows to flag missing years or title breaks.

4. **Data Layer:** The clean, processed timeline is stored in PostgreSQL and sent back to the frontend for visualization.

## 🗺️ Prototype Roadmap (Hackathon Phase)

* \[ \] **Phase 1:** Set up React boilerplate and design the basic user upload flow.

* \[ \] **Phase 2:** Build the FastAPI backend and integrate a basic OCR script for dummy document processing.

* \[ \] **Phase 3:** Develop the Lineage Mapping UI to render the extracted JSON data as a family-tree style timeline.

* \[ \] **Phase 4:** Hardcode edge cases (like a missing signature) to demonstrate the Discrepancy Engine in action for the final pitch.

## 🤝 Team

* **\[Your Name/Team Name\]** - Hackathon Submission for the "Real Estate and Land" Theme.