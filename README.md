# Cold Email Generator
## Overview
The Cold Email Generator is an end-to-end tool designed to help software services companies generate personalized cold emails for potential clients. Using an open-source LLM (Llama 3.1), ChromaDB, and LangChain, this tool extracts job details from potential clients' career pages and composes relevant email responses, thus streamlining the business development process.

## Features
1. Job Posting Extraction: Utilizes LangChain to scrape and parse job postings from company websites.
2. Personalized Cold Email Generation: Llama 3.1 LLM creates custom emails based on job postings.
3. Portfolio Integration: Matches job requirements with existing project portfolios, stored in ChromaDB.
4. Streamlit UI: Offers a user-friendly interface for job posting URL input and email generation.
##Technologies Used
1. Llama 3: Open-source LLM for natural language processing tasks.
2. LangChain: Framework for chaining LLM processes.
3. ChromaDB: Vector database for semantic search.
4. Streamlit: Frontend framework for creating interactive web applications.
5. GroqAPI: Cloud platform for fast LLM inference.
## Setup and Installation
1. Clone the repository:
```bash
git clone <repository-url>
cd cold-email-generator
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Set up environment variables by creating a .env file in the root directory and add your Groq API key:
```bash
GROQ_API_KEY=your_api_key_here
```
4. Start the Streamlit app:
```bash
streamlit run app/main.py
```
## Usage
1. Input a job posting URL in the Streamlit app.
2. The tool scrapes and processes the job posting.
3. The generated email, customized to match the job description and showcase relevant portfolios, will be displayed.
## Project Structure
1. app/: Contains the main application code.
2. resources/: Stores CSV files with portfolio data.
3. utils.py: Utility functions for data cleaning and preprocessing.
4. Chains.py: Handles LLM processes for data extraction and email generation.
5. Portfolio.py: Manages portfolio data in ChromaDB.
6. .csv : constists list of trcstacks and their protfolio websites
### Dependencies
Please refer to the requirements.txt for a complete list of dependencies, including:
1. Llama 3
2. LangChain
3. ChromaDB
4. Streamlit

