Cybersecurity Incident Tracking System
Features

Web Scraping: Extracts cybersecurity incident data from reliable sources.
Machine Learning Classification: Uses TF-IDF + Naive Bayes to categorize incidents into types like Phishing, Ransomware, Malware.
SQLite Storage: Stores all incidents and predictions in a persistent local database.
Insights Generation: Aggregates incident data by type.
Streamlit Dashboard: User-friendly frontend for displaying incidents and insights interactively.

Project Structure
.
├── app.py                    Streamlit frontend
├── scraper.py                Scrapes cybersecurity incidents
├── database.py               Stores scraped data into SQLite
├── ml_classification.py      Classifies incidents using ML
├── insights.py               Generates summary insights
├── cyber_incidents.db        SQLite database file
├── requirements.txt          List of dependencies
└── README.md                 You're here!

Setup Instructions

1. Clone the Repository

bash
git clone https://github.com/ShreeDeepthi/T230_Hackathon
cd cybersecurity-tracker


2. Create a Virtual Environment

bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate


3. Install Requirements

bash
pip install -r requirements.txt


4. Run the Pipeline

1. Scrape data
python scraper.py

2. Store data
python database.py

3. Classify incidents
python ml_classification.py

4. Generate insights (optional)
python insights.py

5. Run Streamlit app
streamlit run app.py


System Architecture -
Website Scraper ──▶ SQLite DB ──▶ ML Classifier ──▶ Insights Generator ──▶ Streamlit UI
Each stage feeds the next, making this a complete ETL + ML visualization pipeline for cybersecurity events.


