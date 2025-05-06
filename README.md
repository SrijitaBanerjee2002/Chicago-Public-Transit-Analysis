# Chicago Public Transport Analysis

**CS 418 – Intro to Data Science**  
**Spring 2025**  
**Team Members**: Srijita Banerjee (Project Lead), Burak Simsek, Heer Patel, Amina Marin, Prince Sonani

---

## Project Overview

This project analyzes trends in Chicago's public transportation system using multi-source data from 2010 to 2024. Our goal was to identify patterns and insights related to:

- CTA **daily ridership trends**
- **Crime incidents** on or near transit lines
- **Public sentiment** based on Reddit posts
- Changes in **security staffing** over time

We combined machine learning, data visualization, and statistical techniques to explore these themes and uncover relationships between public perception, actual events, and system usage.

---

## Repository Structure
├── data/ # Cleaned and processed datasets
├── notebooks/
│ ├── ridership_analysis.ipynb
│ ├── crime_on_crime_ridership.ipynb
│ ├── crime_on_crime_ridership_levels.ipynb
│ ├── reddit_sentiment_analysis.ipynb
│ └── security_staffing_analysis.ipynb
├── figures/ # Generated plots and visuals
├── report/ # Final PDF report submission
└── README.md


---

## Methodology

### CTA Ridership
- Daily total rides from 2010 to 2024 were aggregated and visualized.
- Plotted long-term trends and highlighted pandemic-related drops.
- Crime spike days were overlaid to explore visual associations.

### Crime Correlation
- Flagged statistically significant spike days using z-scores.
- Used scatterplots and regression to evaluate the relationship between daily crime counts and ridership volume.
- Time-slice plots showed local changes around spike days.

### Reddit Sentiment
- Scraped CTA-related Reddit posts.
- Used sentiment scoring (e.g., VADER) to analyze tone across time.
- Compared sentiment patterns to ridership and crime trends.

### Security Staffing
- Parsed security staffing data from FOIA responses.
- Compared guard deployments against crime/ridership levels.
- Visualized annual guard counts and trends.

---

## Tools & Technologies

- **Python** (Pandas, NumPy, Matplotlib, Seaborn, scikit-learn, NLTK, VADER)
- **Jupyter Notebooks**
- **Git/GitHub**
- **JSON/CSV processing**
- **Web scraping & APIs**

---

## Results

- We observed some **inverse trends** between crime spikes and ridership on certain days.
- No strong linear correlation was detected between daily ridership volume and crime counts (as per regression analysis).
- Public sentiment dipped sharply during known crime periods.
- Security staffing showed inconsistencies, with unclear correlation to ridership demand.

---

## Data Sources

- **CTA Ridership Data**: Chicago Transit Authority (CTA)
- **Crime Reports**: City of Chicago Data Portal
- **Reddit Posts**: Scraped via Reddit API (r/chicago, r/cta)
- **Security Staff Data**: Obtained via FOIA requests to CTA

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-team-repo/CS-418-Project.git
   cd CS-418-Project

2. Install dependencies if using requirements.txt
   pip install -r requirements.txt


---

## Acknowledgements
We thank Professor Sourav Medya (medya@uic.edu) and our Teaching Assistants Homaira Huda Shomee (hshome2@uic.edu) and  Peyman Baghershahi (pbaghe2@uic.edu) for their invaluable advice and cooperation throughout the project development process. 



