# Chicago Public Transport Analysis

**CS 418 – Intro to Data Science**  
**Group 2, Spring 2025**  
**Team Members**: Srijita Banerjee (Project Lead), Burak Simsek, Heer Patel, Amina Marin, Prince Sonani

---

## Project Overview

This project analyzes trends in Chicago's public transportation system using multi-source data from 2010 to 2024. Our goal was to identify patterns and insights related to:

- CTA **daily ridership trends**
- **Crime incidents** on or near transit lines
- **Public sentiment** based on Reddit posts
- Changes in **security staffing** over time

We combined machine learning, data visualization, and statistical techniques to explore these themes and uncover relationships between public perception, actual events, and system usage.

### 😊 My Role

As Project Lead, I contributed to overall coordination and direction of the analysis. My primary focus was on:

- Analyzing 14 years of CTA crime data to detect statistically significant spikes using z-score logic
- Merging crime and ridership data to identify behavioral trends in weekday commuter patterns following major crime events
- Creating standalone visualizations and writing the final project report

---

## Repository Structure

```
Project/
├── Collections/                     # Aggregated notebooks & scripts
│   └── security-economic-data.ipynb
├── data/                            # All raw and cleaned datasets
│   ├── CTA_Data/
│   │   ├── CTA_Expenditures/
│   │   │   ├── CTA_Expenditures_2019.csv
│   │   │   ├── CTA_Expenditures_2020.csv
│   │   │   └── ...                 
│   │   ├── CTA_Crimes_2010.csv
│   │   ├── CTA_Crimes_2011.csv
│   │   └── ...
│   └── Other_Data/
│       ├── Employee_Overtime_and_Support.csv
│       └── ...
├── crime_analysis.ipynb             # General crime trend exploration
├── crime_on_crime_ridership_levels.ipynb  # Deep dive into crime spikes vs ridership
├── cta_data.ipynb                   # Initial CTA data parsing and filtering
├── rider_sentiment.ipynb           # Reddit sentiment analysis
├── reddit_comments.csv             # Raw Reddit data
├── reddit_sentiment.csv            # Labeled sentiment scores
├── progress_report.ipynb           # Intermediate notebook to document progress
├── security-staffing-trends.ipynb  # CTA staff and safety budget analysis
```




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
   ```bash
   pip install -r requirements.txt


---

## Acknowledgements
We thank Professor Sourav Medya (medya@uic.edu) and our Teaching Assistants Homaira Huda Shomee (hshome2@uic.edu) and  Peyman Baghershahi (pbaghe2@uic.edu) for their invaluable advice and cooperation throughout the project development process. 

---

## 🙋‍♀️😊 About Me
Hi! I’m Srijita Banerjee, a recent Computer Science graduate from UIC passionate about applying ML to meaningful, real-world problems.  
This project was an early but important step in my journey into machine learning, and I’m proud of what we built as a team.

📫 [Reach out to me](mailto:banerjeesrj@gmail.com) or connect via [LinkedIn](https://www.linkedin.com/in/srijitabanerjee)



