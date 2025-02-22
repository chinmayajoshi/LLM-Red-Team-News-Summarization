# News Summarization Bot: Automated Red Team Scan

This repository contains news summarization bot with AI security analysis (Red Team) project using Giskard, LangChain and Google Gemini LLMs. It performs automated security scans using `Giskard` with `Gemini 2.0 Flash` LLM, and exports reports in [AI Vulnerability Database (AVID)](https://docs.giskard.ai/en/latest/integrations/avid/index.html) format.

## Repository Structure

| File                                       | Description                                                                                    |   
| ------------------------------------------ | ---------------------------------------------------------------------------------------------- | 
| **Newspaper\_Summary\_Red\_Team\_Scan.ipynb**  | Jupyter Notebook implementing news summarization and AI security scans using LangChain and Giskard. |   
| **avid\_report.jsonl**                     | AI Vulnerability Database (AVID) reports in JSONL format.                                      |  
| **AI\_Vulnerability\_JSON\_Reports.ipynb** | Notebook for reading and processing AVID reports.                                              |   
| **Giskard Scan Report Screenshot.jpg**     | Screenshot showcasing a Giskard security scan report.                                          |   

## Setup and Dependencies

### Install Required Packages

Ensure you have the necessary dependencies installed by running:

```bash
pip install "giskard[llm]" langchain-google-genai avidtools pillow
```

### API Keys

- The project requires API access to Google Gemini for LangChain processing.
- Ensure you set up `GEMINI_API_KEY` in your environment.

## Identified Vulnerabilities

Giskard Red Team Vulnerability Scan Screenshot below:

- Harmfulness
![img](images/Giskard_Scan_Report_Screenshot_1.jpg "Giskard Vulnerabilities Scan #1")

- Sensitive Data Disclosure
![img](images/Giskard_Scan_Report_Screenshot_2.jpg "Giskard Vulnerabilities Scan #2")


The interactable Giskard Scan is not viewable on `ipynb` files uploaded on `Github`.<br>
Checkout the same [Google Colab notebook](https://colab.research.google.com/drive/1KMKo-3yHC-RX82JrMtBWDllAl-XWVzQW) to interact with the above Giskard Scan in-detail.

## Acknowledgments

- [Giskard AI Security](https://giskard.ai)
- [AI Vulnerability Database (AVID)](https://avidml.org)