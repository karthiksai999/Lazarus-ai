Dead Code Detector:

An AI-powered tool to find and explain unused code in Python and JavaScript projects.

---

What it does:-

- Detects unused functions, unread variables, and unreachable statements
- Works across multiple files — not just single files
- Gives AI-generated explanations (LLaMA 3) for every issue found
- Shows an interactive call graph of your code
- Gives your project a Code Health Score

Tech Stack:-

- Frontend — React, Monaco Editor, Cytoscape.js
- Backend — FastAPI, Python AST
- AI — Groq API + LLaMA 3

Getting Started:-

Backend
- cd backend
- pip install -r requirements.txt
- export GROQ_API_KEY=your_key_here
- uvicorn main:app --reload

Frontend
- cd frontend
- npm install
- npm start

How it works:-

1. Paste or upload your code
2. The system builds an AST and finds all definitions vs usages.
3. Anything defined but never used is flagged as dead code.
4. LLaMA 3 explains why it's dead and how to fix it.
5. Results show up as a list + call graph + health score.

Results:-

 Metric              Value 
- Detection Accuracy: 95% 
- Analysis Time: 1–2 sec per file
- False Positives:  Low 
