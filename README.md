![Project-logo](https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/raw/main/project-logo.png)

## Project title: Stack overflow software developer survey analysis (Big Data Analysis)  
  
## Project description  
This project is dedicated to a detailed analysis of the results of the annual Stack Overflow Developer Survey 2025. The purpose of the analysis is to study current trends in the IT industry, investigate the popularity of the Python language, and analyze the factors influencing the high compensation of remote workers.  

## Data used  
The analysis used open data from the annual Stack Overflow Developer Survey 2025.  
  **Source:** [Stack Overflow Insights](https://survey.stackoverflow.co/)  
  **Sample size:** Over 49,000 respondents from around the world.  
  **Data composition:** The file contains developer responses about technology stack (languages, frameworks), income level, work format (Remote/Office), education, and demographics.  

## Technology stack  
**Language:** Python 3.12  
**Libraries:** Pandas (data processing), Matplotlib & Seaborn (visualization), Plotly (interactive graphs).  
**Environment:** Google Colab.  

## Key stages of analysis  
  **1. Pre-processing:** Data cleaning and normalization.  
  **2. Data Export:** The processed and cleaned dataset is saved to a separate file survey_results_cleaned.csv for further use in other studies.  
  **3. Demographic portrait:** Analysis of work experience (WorkExp) and age categories.  
  **4. Python ecosystem:** Study of language popularity among different groups and analysis of median salaries.  
  **5. Remote Work:** Filtering of highly paid professionals (Top 25% by income) and their distribution by industry.  

## Key insights  
 - **Python dominates:** 37.5% of respondents use Python, with the peak popularity occurring in younger age groups.  
 - **Community Experience:** The median developer experience is 10 years, indicating a mature market.  
 - **Education:** Over 43% of professionals use online courses as their primary source of knowledge, highlighting the flexibility of today’s IT education.  
 - **High-Paid Industries:** The highest salaries for remote work are concentrated in the Software Development, Fintech, and Healthcare sectors.  

 ## Visualizations  
The project includes:  
 - Histograms of experience distribution.
  
![Experience Distribution](https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/raw/main/results/work_experience_dist.png)
  
 - Comparative charts of "Median vs Mean" salaries by country.
  
![salaries by country](https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/raw/main/results/python_median_vs_mean.png)
  
 - Donut-chart of distribution of work formats (Remote/Hybrid/In-person).
  
![Analysis image 1](https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/raw/main/results/remote_work_pie_chart.png)
  
- Python popularity trends by age.
  
![Analysis image 1](https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/raw/main/results/python_popularity_by_age.png)  
  
## Project structure

**Stack-overflow-software-developer-survey-analysis/** — project directory  
    | - data/ — project data  
    |     | - raw/ — raw data  
    |     | - processed/ — cleaned data  
    | - notebooks/ — main file with analysis code (Project_0001p.ipynb)  
    | - reports/ — report of project  
    | - results/ — saved graphs and final tables    
    | - requirements.txt — list of libraries to run the project  
    | - .gitignore - git ignore patterns  
    | - LICENSE — license file  
    | - project-logo.png — project cover  
    | - README.md — project description  
  
## How to Use  
  
**How to use this project**  
To run this analysis locally, follow these steps:  
  
**1. Download the project file**  
  
[project-notebook.ipynb](https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/blob/main/notebooks/project-notebook.ipynb)  
  
File location: https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/blob/main/notebooks/project-notebook.ipynb  
  
**2. Download the dataset**
  
[stack-overflow-developer-survey-2025.zip](https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/blob/main/data/raw/stack-overflow-developer-survey-2025.zip)  

File location:  
https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/blob/main/data/raw/stack-overflow-developer-survey-2025.zip  

The data is large, so it was previously archived.  
  
Archive content:  

**survey_results_public.csv** — the main anonymized responses of respondents (the primary object of analysis).  
**survey_results_schema.csv** — explanation of column headings and question texts.  
**2025_Developer_Survey_Tool.pdf** — the complete survey structure for understanding the context of data collection.  
  
Alternative way to obtain data:  

https://survey.stackoverflow.co/  

**3. Running the analysis**
  
You can open the notebook in Jupyter Notebook, VS Code, or upload it to Google Colab:  
  
• **For Jupyter:** jupyter notebook notebooks/project-notebook.ipynb  
• **For Colab:** simply upload the Project_0001p.ipynb file to your Google Drive.  
  
To connect the dataset to the project locally in step 1. "Data acquisition" of the project, replace the path to the **survey_results_schema.csv** and **survey_results_public.csv** files with the current one  
    
**Was:**  
srs_df_url = '/content/drive/MyDrive/ISAO/data/survey_results_schema.csv'  
srp_df_url = '/content/drive/MyDrive/ISAO/data/survey_results_public.csv'  
  
**Now:**   
srs_df_url = 'path to file /survey_results_schema.csv'  
srp_df_url = 'path to file /survey_results_public.csv'  
  
## Contact  
    
**Name:** Andrii Isachenko  
**LinkedIn:** [Andrii Isachenko](https://www.linkedin.com/in/isachenko-andrii/)  
**E-mail:** isao.datastudio@gmail.com   
  
## Acknowledgments    
 
 - Thanks to the [Stack Overflow](https://survey.stackoverflow.co/) community for the open data.  
 - Thanks to the [Data Analyst/GoIT](https://goit.global/ua/courses/data-analytics/) course, which was part of this project.

---
  
**Project Status:** Completed. In the future, we plan to add analysis of the correlation between the use of AI tools and income level. Anomaly analysis - conducting a detailed study of the outliers segment.  
    
**License:** MIT License.



