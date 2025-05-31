# MediMind - Clinical AI Assistant for Doctors

**MediMind** is a Streamlit web application powered by the `LLaMA 3` language model via `LangChain`. It is designed to assist medical professionals in analyzing patient case data and providing expert-level clinical decision support, including symptom analysis and recommended actions.

---

## Features

- **Symptom Analysis**: Returns differential diagnoses with percentage likelihood.
- **Clinical Decision Support**: Suggests immediate actions, medications, and follow-ups.
- **Case Data Logging**: Saves patient data and AI response to a CSV file.
- **Interactive UI**: User-friendly form interface for entering patient details.

---

## Requirements

Ensure you have the following installed:

- Python 3.8+
- [Streamlit](https://streamlit.io/)
- [Pandas](https://pandas.pydata.org/)
- [LangChain](https://python.langchain.com/)
- [Ollama](https://ollama.com/) (for local LLaMA model support)

You can install the required libraries with:

```bash
pip install streamlit pandas langchain

ollama run llama3

##Project Structure

medimind/
│
├── medical_assistant_llm.py                # Streamlit application code
├── patient_cases.csv     		     # Saved case records (auto-created)
└── README.md             		     # Project documentation

##Library_versions:
streamlit                 1.45.0
pandas                    2.2.3
langchain-community       0.3.24



##How to Run
Start Ollama and ensure the llama3 model is available:

bash
Copy
Edit
ollama run llama3
Run the Streamlit app:

bash
Copy
Edit
streamlit run app.py
Open your browser and go to http://localhost:8501 to use MediMind.

##Usage Instructions
Enter patient information (name, age, gender, etc.).

Provide clinical data: symptoms, medical history, test results.

Submit a physician query (e.g., "What’s the diagnosis and next steps?").

View the AI-generated analysis and save the data automatically.

##Output
Each analysis includes:

Differential Diagnoses with % likelihood.

Recommended actions like diagnostics, treatments, or referrals.

All inputs and outputs are stored in patient_cases.csv.

##Disclaimer
This tool is for educational and research purposes only and is not intended to replace professional medical judgment. Always consult a licensed healthcare provider for clinical decisions.

