# Threat by Association
*A Corpus-Based Analysis of the Discursive Criminalization of Migrants and Displaced Communities*  

Malorie Iovino  
MSc Candidate in Computational Linguistics, Goldsmiths, University of London  

Prepared for **AMLI 2025 Conference**
Liverpool Hope University, September 2025

---

##  Overview
This repository contains the paper and presentation slides for my AMLI 2025 conference project, Threat by Association. The research investigates how Western, English-language media discursively constructs displaced populations, criminalizing some groups while humanizing others.

Using a mixed-methods framework that combines computational linguistics with Critical Discourse Analysis (CDA), the study explores how lexical choices, and grammatical constructions function as ideological tools. 

---

## Research Question 
How do Western media outlets use linguistic choices to construc displaced people differently across racial, religious, and geopolitical identities?

---

## Key Contributions 
- **Corpus-based evidence:** Analysis of 1,700+ articles from CNN and The Guardian (2021–2025), plus partisan outlets (Fox News, Daily Mail, New York Times, The Independent).
- **Computational methods:**
  - Collocation and frequency analysis
  - Part-of-speech tagging and transitivity analysis
  - Comparative distributions of evaluative adjectives + verbs
- **Critical Discourse Analysis (CDA):**
  - Headlines + URL framing
  - Case studies covering *Anas al-Sharif* and *Kilmar Abrego Garcia*
- **Findings:**
  - Palestinians are framed as passive victims—grievable but denied agency.

  - Ukrainians are portrayed as complex humans, balancing victimhood with rational action.

  - Latin Americans are discursively reduced to administrative problems or criminalized as threats.

These framings map onto proximity to whiteness, religion, and geopolitical alignment with Western interests. 

This work highlights how journalism functions as a form of linguistic border control, actively shaping public perception, legitimizing policy, and determining whose lives are rendered visible and grievable.  

---

##  Repository Structure
```plaintext
docs/
  ├── threat_by_association.pdf        # Final paper
  └── amli_threat_by_association_slides.pptx  # Conference slides

scripts/
  ├── cnn_corpus.py
  ├── data_collection.py
  └── evaluation.py

data/
  ├── cnn_guardian_corpus.csv
  └── supplementary.csv

figures/
  ├── collocation_plot.png
  └── agency_analysis.png
```
## Methods
- **Corpus Construction:**
  - CNN articles via GDELT + scraping
  - Guardian articles via Open Platform API
  - Supplementary partisan outlets (Fox News, Daily Mail, New York Times, The Independent)
- **Analytical Tools:**
  - Lexical choice analysis
  - Collocation patterns (5-word windows, log-likelihood)
  - Transitivity analysis (Halliday's SFG)
  - CDA with focus on metaphor, nominalization, and agency
    
## How to Run 
**1. Clone the repo**
```
git clone https://github.com/malorieiovino/threat-by-association.git
cd threat-by-association
```
**2. Install dependencies**
```
pip install -r requirements.txt
```
**3. Run the analysis scripts:** 
```
python scripts/data_collection.py
python scripts/cnn_corpus.py
python scripts/evaluation.py
```
