# Threat by Association
*A Corpus-Based Analysis of the Discursive Criminalization of Migrants and Displaced Communities*  

Malorie Iovino  
MSc Candidate in Computational Linguistics, Goldsmiths, University of London  

---

##  Abstract
This project examines how Western, English-language media constructs displaced populations through systematic linguistic strategies that criminalize some groups while humanizing others. Using a mixed-methods approach that combines computational linguistics with Critical Discourse Analysis (CDA), the study analyzes coverage from mainstream and partisan outlets to reveal how discourse operates unevenly across racial, religious, and geopolitical contexts.  

Key findings:
- **Palestinians** are trapped in passive grammatical constructions that deny agency.  
- **Latin Americans** are dehumanized through metaphors (e.g., “floods,” “invasions”).  
- **Ukrainians** receive balanced framing that preserves both vulnerability and rational action.  

This work highlights how journalism functions as a form of linguistic border control, actively shaping public perception, legitimizing policy, and determining whose lives are rendered visible and grievable.  

---

##  Repository Structure
```plaintext
docs/
  ├── threat_by_association.pdf        # Final paper
  ├── amli_threat_by_association_slides.pptx  # Conference slides
  └── drafts/
      └── AMLI Draft (9).pdf           # Earlier draft

scripts/
  ├── cnn_corpus.py
  ├── data_collection.py
  └── evaluation.py

data/
  ├── sample_corpus.csv (optional)
  └── processed/ (shareable processed data)

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
