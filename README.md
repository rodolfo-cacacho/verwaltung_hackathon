# KURVE – KI-unterstützte Recherche und Verarbeitung von Stellungnahmen

This repository contains our solution for the **KURVE Hackathon Project**, developed in collaboration with **THWS Master AI Würzburg**.  
The goal is to support public administrations by automating the analysis and summarization of large volumes of non-formally structured public statements.

## 🧠 Problem Statement: Automating the Processing of Public Statements

Public authorities frequently receive thousands of statements during public participation procedures (sometimes up to 100,000). These must be reviewed individually, which is time-consuming and inefficient. Many statements are redundant or off-topic, and manual processing leads to delays.

### Key Challenges
- Reading documents in PDF format, including OCR and handwritten content.
- Separating and identifying individual complaints/statements.
- Clustering and summarizing content while removing redundancy.
- Ensuring traceability from summaries back to individual sources.
- Anonymizing sensitive or personal data.
- Generating structured "consideration documents" for planning authorities.
- Guaranteeing data protection throughout the entire process.

## 💡 Our Solution

We built an AI-assisted pipeline that extracts, processes, and summarizes the main points from each submitted statement, providing a scalable and semi-automated solution to accelerate public administration workflows.

### 🧾 Document Processing

- Input documents were provided in **PDF format**.
- Each PDF was **parsed and segmented** into individual **complaints/statements**.
- Text-based PDFs were supported.

### 🧹 Anonymization with NER

- We used **Named Entity Recognition (NER)** to detect and anonymize **personally identifiable information**.

### 📚 Clustering & Summarization with LLAMA3

- We used **LLAMA3** to generate **summaries** of the complaints.
- Semantic **clustering** was performed to group similar complaints (based on content and topic).
- Clusters were processed into concise summaries, ensuring all concerns were addressed without redundancy.

### 📄 Output: Consideration Document

- The final result is a structured **summary document**, grouped by:
  - Thematic content (e.g., water, forests, traffic)
  - Specific project areas
  - Special or individual concerns
- Each summary links back to the relevant original complaint(s) to ensure **traceability**.

### ✅ Impact

Our pipeline significantly reduces the **manual workload** and **processing time** required to evaluate public statements. It also increases the **transparency** and **consistency** of the evaluation process.

🤖 Technologies Used
	•	LLAMA3 for text generation and summarization
	•	Named Entity Recognition for anonymization
	•	PDF parsing

📫 For any questions, feel free to reach out!
