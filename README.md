🏥 ClinCode
Resolving Clinical Ambiguity with Explainable AI

An intelligent system that converts unstructured doctor notes into accurate ICD-10 codes — with reasoning, confidence, and ambiguity detection.

🚀 Overview

ClinCode is designed to solve a critical problem in healthcare:

Doctors write ambiguous and incomplete notes, while ICD-10 coding requires highly specific structured information.

This mismatch leads to:

Incorrect coding
Financial losses
Lack of trust in automation

ClinCode addresses this by treating coding as an uncertainty resolution problem, not just a classification task.

💡 Key Features
🧠 Clinical NLP Understanding
Extracts diseases, symptoms, and medical entities from text
⚠️ Ambiguity Detection (Core USP)
Identifies missing or unclear information before coding
🤖 Smart ICD-10 Mapping
Suggests multiple possible codes with confidence scores
💬 Interactive Clarification
Asks follow-up questions to resolve uncertainty
🔍 Explainable AI
Shows exactly why each code was selected
🔁 Feedback Loop
Learns from corrections to improve over time
⚙️ System Architecture
Input (Doctor Notes)
        ↓
Preprocessing (Normalization, Abbreviation Expansion)
        ↓
Medical Entity Extraction (BioBERT / ClinicalBERT)
        ↓
Context & Relationship Modeling
        ↓
Ambiguity Detection Engine
        ↓
ICD-10 Inference Engine
        ↓
Explainability Layer
        ↓
Output (Codes + Confidence + Reasoning)
🔬 Example
Input:
Patient has diabetes with kidney issues and proteinuria
Output:
E11.65 → Type 2 Diabetes with complications (87%)
N18.3 → Chronic Kidney Disease Stage 3 (91%)
E11.69 → Alternative code (22%)

✔ Explanation:

Diabetes + kidney issue → linked complication
Proteinuria → strengthens kidney diagnosis


🧠 Core Innovation



Instead of blindly predicting codes, ClinCode detects ambiguity, resolves it, and explains decisions.



🛠️ Tech Stack
AI / NLP
BioBERT / ClinicalBERT (HuggingFace)
scispaCy (entity + dependency parsing)
NegSpacy (negation detection)
SapBERT + FAISS (ICD similarity search)
Backend
Python
FastAPI
Frontend
Next.js / React


🔥 Why This Project Stands Out
Traditional Systems	ClinCode
Direct prediction	Reasoning-based system
Ignores ambiguity	Detects & resolves ambiguity
Black-box output	Fully explainable
Single code	Ranked codes with confidence


🎯 Impact
Improves coding accuracy
Reduces manual workload
Builds trust in AI for healthcare
Prevents costly billing errors


🧪 Future Improvements
Integration with hospital EHR systems
Better clinical dataset fine-tuning
Real-time doctor assistant interface
Continuous learning from user feedback





👨‍💻 Authors
Rudra Pratap Singh
Team Antigravity
SRM Institute of Science and Technology
