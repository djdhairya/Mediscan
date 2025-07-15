# MediScan 

## Overview

MediScan is an intelligent web application and command-line tool for analyzing medical case reports using AI-powered agents. It simulates the expertise of a Cardiologist, Psychologist, and Pulmonologist, then combines their insights for a multidisciplinary diagnosis. The project is designed to help healthcare professionals and researchers streamline the review of medical reports.

## Features

- Upload `.txt` medical reports via a web interface
- AI agents simulate specialist reviews (Cardiology, Psychology, Pulmonology)
- Multidisciplinary team agent combines specialist insights for a final diagnosis
- Results saved to `results/Final_Diagnosis.txt`
- User-friendly web interface built with Flask and Tailwind CSS
- Command-line script for batch processing

## How It Works

1. **Upload or select a medical report** (`.txt` file).
2. **AI agents** (Cardiologist, Psychologist, Pulmonologist) analyze the report in parallel.
3. **Multidisciplinary Team agent** synthesizes the findings for a comprehensive diagnosis.
4. **Diagnosis is saved** to `results/Final_Diagnosis.txt` and displayed in the web interface.

## Project Structure

```
Mediscan/
│
├── app.py                  
├── main.py                
├── Utils/
│   └── Agents.py           
├── doc/
│   ├── Medical_Report.txt
│   ├── Medical_Report_1.txt
│   └── Medical_Report_2.txt
├── uploads/                
├── results/
│   └── Final_Diagnosis.txt 
└── templates/
    └── index.html          
```

## Getting Started

### Prerequisites

- Python 3.12+
- [Flask](https://flask.palletsprojects.com/)
- [langchain](https://python.langchain.com/)
- [langchain_groq](https://github.com/langchain-ai/langchain-groq)

### Installation

1. **Clone the repository:**
    ```sh
    git clone https://github.com/djdhairya/Mediscan.git
    ```

2. **Install dependencies:**
    ```sh
    pip install flask langchain langchain_groq
    ```

3. **Set up your Groq API key** in `Utils/Agents.py` as required.

### Usage

#### Run the Web App

```sh
python app.py
```
- Visit [http://localhost:5000](http://localhost:5000)
- Upload a `.txt` medical report
- View the AI-generated diagnosis

#### Run from Command Line

```sh
python main.py
```
- Processes a sample report and saves the diagnosis to `results/Final_Diagnosis.txt`

## Customization

- Modify agent prompts in `Utils/Agents.py`
- Update HTML/CSS in `templates/index.html`
- Add more specialist agents as needed

## About MediScan 

MediScan  aims to assist clinicians and researchers by providing rapid, multidisciplinary assessments of medical case reports. Its modular design allows for easy expansion and integration of additional specialties or custom diagnostic logic.



<img width="1913" height="909" alt="Screenshot 2025-07-15 153301" src="https://github.com/user-attachments/assets/394516c6-5f9c-449e-8dbf-3671ea334f59" />

<img width="1109" height="734" alt="Screenshot 2025-07-15 153328" src="https://github.com/user-attachments/assets/2c20d91f-ec0c-4b47-9e5c-734252a229ff" />

