# AIMScribe_NLP
Clinical Protocol RAG Recommendation Prototype
1. Overview & Model Details
•	Project Type: Clinical Decision Support System (CDSS) prototype using Retrieval-Augmented Generation (RAG). 
•	User Interface: Interactive web application built with Gradio. 
•	Knowledge Retrieval: Term Frequency–Inverse Document Frequency (TF-IDF) vectorizer with unigram and bigram tokenization calculating cosine similarity against indexed protocol cards. 
•	Language Model: Qwen/Qwen2.5-1.5B-Instruct (loaded locally from HuggingFace via PyTorch and Transformers with device_map="auto", temperature=0.1, and deterministic greedy generation via do_sample=False). 
•	Medical Knowledge Base: canonical_cards.json containing 19 canonical clinical protocol cards extracted from official Bangladeshi and WHO guidelines (covering Dengue, Hypertension, Cholera, and Chikungunya). 
2. Environment Setup & Launch Instructions
Execution Platform
The entire system was developed, executed, and evaluated within a Kaggle Notebook environment. It runs self-contained without requiring external cloud API keys, paid tokens, or external network calls. 
Python Dependencies
Run the following installation command in your notebook or local environment: 
pip install gradio scikit-learn transformers accelerate torch numpy
Launch Steps in Kaggle Notebook
1.	Place canonical_cards.json in the active working directory (/kaggle/working/). 
2.	In the right-hand Kaggle settings sidebar, toggle Internet to ON (required to download the open-weights model from HuggingFace on the initial run). 
3.	For best speed, set the Accelerator to GPU T4 x2 (runs in 2–3 seconds per query; CPU is supported but slower). 
4.	Run the notebook cells sequentially from top to bottom. 
5.	The Gradio interface renders automatically inside the notebook output and generates a public URL (https://<hash>.gradio.live) for live remote testing. 
Standalone Local Execution
If running locally as a script: python app.py
3. RAG Index & Rebuild Instructions
The knowledge index is built dynamically in-memory directly from canonical_cards.json. 
•	Vector Representation: Each card's title, disease, clinical category, prerequisites, recommended actions, exclusions, and verbatim guideline evidence passage are concatenated into an indexed corpus string. 
•	Rebuilding: The TF-IDF sparse matrix is fitted in fewer than 50 milliseconds at startup. To update the clinical knowledge base, simply edit or append cards inside canonical_cards.json and re-run the notebook or script. No external vector database server (such as Pinecone, Chroma, or Milvus) is required. 
4. Evaluation Modes (Baseline vs. Improved)
The Gradio web interface features an "Engine Mode" radio switch allowing the examiner to toggle between two operational modes on any patient case: 
1.	Baseline Mode:
•	Retrieves the top 4 matching cards strictly by overall TF-IDF cosine similarity score. 
•	Passes the retrieved text directly to the model with standard evidence-grounding instructions. 
2.	Improved Mode:
•	Category-Balanced Retrieval: Guarantees balanced clinical representation by pulling the highest-scoring card from each of the 4 clinical categories (probable_diagnosis, investigations, medication_guidance, and advice), plus the top 2 remaining conditional or differential cards (6 cards total). 
•	Safety Verification Prompt Gate: Instructs the language model to verify patient age, pregnancy status, and comorbidities against card prerequisites before formatting the medication plan (e.g., blocking Losartan in pregnant women). 
5. Repository File Manifest
File Name	Description
README.md	System overview, environment setup, model details, and execution instructions. 
canonical_cards.json	19 canonical JSON cards covering Dengue, Hypertension, Cholera, and Chikungunya protocols. 
Notebook	Complete runnable source code containing the RAG retriever, Qwen model loader, and Gradio interface. 
six_cases_and_12_outputs.json	Machine-readable JSON export of all 6 fictional cases executed across both Baseline and Improved modes (12 outputs total). 
six_cases_and_12_outputs.md	Human-readable Markdown export of the 12 saved engine outputs including response times and card summaries. 
Complete_Written_Report	Contains:
1.	Question1Explanation.pdf
2.	Question2Checklists.pdf
3.	Question3Architecture.pdf
4.	Question4PaperReport.pdf 
NLP Diagram.drawio.png	High-resolution end-to-end system architecture diagram. 
Presentation_Slides.pdf	10-minute presentation slides. 
6. Disclosure of Tools & AI Assistance
•	Libraries & Models: Python 3, PyTorch, HuggingFace Transformers, Scikit-Learn, Gradio, NumPy. 
•	Hardware Environment: Kaggle Notebooks. 
•	Architecture Diagram: Draw.io. 
•	AI Tool Disclosure: An AI assistant (Google Gemini) was consulted for troubleshooting environment timeouts, formatting Gradio UI components, and checking JSON syntax. All clinical rule extractions from the 45 assigned protocol pages, canonical JSON cards, case scenario designs, and evaluation verifications were manually authored and checked against the source medical guidelines. 

