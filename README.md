# AI/ML Job Market Explorer (India + Remote)

## Why I built this
I'm preparing for ML/AI Engineer, Agentic AI, and LLM Engineer roles and wanted 
real data on what skills, tools, and experience levels are actually being asked 
for — instead of guessing from a handful of job descriptions.

## A note on the data source
I originally set out to scrape live postings from Naukri.com. I got as far as 
finding their internal JSON API via DevTools Network tab (cleaner than parsing 
HTML), but hit a hard wall: the API requires a signed request token and, on 
repeated calls, returns a 406 reCAPTCHA-required response — a deliberate 
anti-bot measure. Rather than go down the path of CAPTCHA workarounds or full 
browser automation to evade detection, I made the call to use a pre-existing 
Kaggle dataset instead, since my actual goal is EDA and analysis depth, not 
adversarial scraping.

## What it does
Explores a dataset of AI/ML job postings to surface patterns in:
- Most in-demand skills and tools
- How requirements differ by experience level
- [Add more as you finalize your analysis angles]

Built as an interactive Streamlit app so the analysis is explorable, not just 
static charts.

## Status
In progress — learning project, updated as I go.
Currently: [e.g. "dataset loaded, cleaning in progress"]

## Tech stack
Python, pandas, Seaborn, SQL, Streamlit

## How to run
bash
pip install -r requirements.txt
streamlit run app.py


## What I found (updated as project progresses)
- [Insight 1, with chart reference]
- [Insight 2]
- [Insight 3]

## What I'd improve next
- [Honest self-critique — e.g. "dataset is a snapshot, not live — a future 
  version could revisit live scraping with proper API access or a friendlier 
  source"]

## Project structure
job-market-eda/  
  data/raw/          # kaggle dataset 
  data/processed/    # cleaned data[CSV file]
  notebooks/eda.ipynb  
  src/    
    clean.py  
  outputs/figures/
