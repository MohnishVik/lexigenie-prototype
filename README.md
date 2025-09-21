# LexiGenie: AI-Powered Legal Document Analysis (Hackathon Prototype)

LexiGenie is a pioneering AI platform designed to make complex legal documents clear, accessible, and actionable. This repository contains the functional prototype developed for the GenAI Exchange Hackathon.

## Mission
Our mission is to close the global accessibility gap in legal understanding, starting with the Indian market. By leveraging the power of generative AI, we transform dense legal jargon into simple summaries, identify hidden risks, and empower users to negotiate fairer terms.

## Features Showcased in This Prototype
This prototype is a single, self-contained HTML file that demonstrates the core "magic loop" of LexiGenie. It is fully interactive and built to showcase our vision in a compelling, 3-minute demo.

- Seamless Document Upload: A clean, captivating UI that accepts .txt, .pdf, and .docx files via click or drag-and-drop.  
- Live & Demo Analysis Modes:  
  - Live AI Analysis: For .txt files, the prototype makes a real-time call to the Gemini API to perform a dynamic analysis.  
  - Demo Mode: For .pdf and .docx files, it uses high-quality, pre-built sample data to ensure a flawless and impressive demonstration every time.  
- Instant Legal Health Score: An animated gauge provides an immediate, at-a-glance rating of the document's fairness.  
- In-Depth Risk Radar: Identifies and explains high-risk clauses (e.g., "Strict Lock-in Period"), color-coding them by severity.  
- Data-Driven Benchmark Comparison: Elevates the analysis by comparing clauses in the user's document against common practices in the Indian market.  
- AI Redlining: A direct call to the Gemini API suggests fairer, more balanced wording for risky clauses.  
- Actionable Email Generation: Empowers the user by instantly generating a professional negotiation email draft for any identified risk.  
- Interactive Q&A: Allows users to ask follow-up questions about the document, receiving concise answers from the AI.  

## Technology Stack
This prototype is built with a lean and modern stack, designed for rapid development and a stellar user experience.

- Frontend: HTML5, Tailwind CSS  
- Logic & Interactivity: Vanilla JavaScript (ES6+)  
- Generative AI: Google's Gemini API (gemini-2.5-flash-preview-05-20)  

## Getting Started: Running the Prototype Locally
This project is a single HTML file and is incredibly easy to run on your local machine using Visual Studio Code.

### Prerequisites
- Visual Studio Code  
- Live Server Extension for VS Code  

### Steps
1. Set Up the File  
   Simply open your index.html file directly in VS Code.  

2. Install Live Server in VS Code  
   - Open VS Code.  
   - Go to the Extensions view (click the icon with four squares in the sidebar).  
   - Search for Live Server by Ritwick Dey.  
   - Click Install.  

3. Add Your Gemini API Key (Crucial Step)  
   - Get your free key from Google AI Studio.  
   - In the index.html file, scroll to the bottom to find the `<script>` section.  
   - Find the line:  
     ```javascript
     const API_KEY = "";
     ```  
   - Paste your key inside the quotes:  
     ```javascript
     const API_KEY = "YOUR_API_KEY_HERE";
     ```  
   - Note: The demo mode for .pdf and .docx files will work perfectly even without an API key, making it ideal for a quick demonstration.  

4. Run the Prototype  
   - Right-click anywhere inside your index.html file in the VS Code editor.  
   - Select "Open with Live Server" from the context menu.  
   - Your default browser will open with the LexiGenie prototype running flawlessly, ready for you to record your demo video.  

## Prototype vs. The Final Vision
This prototype is a powerful proof-of-concept. The final project will expand on this foundation to become a comprehensive, nation-scale platform.

| Feature              | This Prototype                         | Final Project Vision                                |
|----------------------|-----------------------------------------|----------------------------------------------------|
| Backend              | JavaScript (Client-side logic)         | Robust Python backend (Flask/FastAPI)              |
| Document Parsing     | Simulates PDF/DOCX; reads .txt          | Google Document AI for high-accuracy OCR on all formats |
| Benchmarking         | Hardcoded sample data                  | Live queries to a BigQuery dataset of contracts    |
| Accessibility        | Web Application                        | Multi-channel via WhatsApp and Voice Assistants (Dialogflow CX) |
| Integrations         | Standalone                             | Google Workspace (Gmail, Drive) for auto-analysis  |
| Collaboration        | Single-user                            | "Lawyer-in-the-Loop" for expert consultation       |

## Vision
We believe LexiGenie has the power to democratize legal literacy, starting in India and scaling globally.
