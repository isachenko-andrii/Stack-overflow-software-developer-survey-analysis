![Project-logo](https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/raw/main/project-logo.png)
#### [EN](https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/blob/main/README.md) | [UA](https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/blob/main/README-UA.md) Цей матеріал також доступний англійською мовою.
---  
<div align="center">  
    
## Stack overflow software developer survey analysis<br>(Big Data Analysis)   
  
</div>  
  
## Опис проєкту  
Цей проєкт присвячений детальному аналізу результатів щорічного опитування розробників Stack Overflow 2025. Метою аналізу є вивчення сучасних тенденцій в ІТ-індустрії, дослідження популярності мови Python та аналіз факторів, що впливають на високу компенсацію віддалених працівників. 

## Використані дані  
В аналізі використовувалися відкриті дані з щорічного опитування розробників Stack Overflow 2025.  
  **Джерело:** [Stack Overflow Insights](https://survey.stackoverflow.co/)  
  **Розмір вибірки:** Понад 49 000 респондентів з усього світу.  
  **Склад даних:** Файл містить відповіді розробників щодо технологічного стеку (мови, фреймворки), рівня доходу, формату роботи (віддалено/офіс), освіти та демографічних показників. 

## Технологічний стек   
**Мова:** Python 3.12  
**Бібліотеки:** Pandas (обробка даних), Matplotlib & Seaborn (візуалізація), Plotly (інтерактивні графіки).  
**Середовище:** Google Colab.  

## Ключові етапи аналізу 
  **1. Попередня обробка:** Очищення та нормалізація даних.  
  **2. Експорт даних:** Оброблений та очищений набір даних зберігається в окремому файлі survey_results_cleaned.csv для подальшого використання в інших дослідженнях.  
  **3. Демографічний портрет:** Аналіз досвіду роботи (WorkExp) та вікових категорій.  
  **4. Екосистема Python:** Дослідження популярності мов серед різних груп та аналіз медіанних зарплат.  
  **5. Віддалена робота:** Фільтрування високооплачуваних фахівців (топ-25% за рівнем доходу) та їх розподіл за галузями.  

## Ключові висновки  
 - **Пітон домінує:** 37,5% респондентів використовують Python, причому пік популярності припадає на молодші вікові групи.  
 - **Досвід громади:** Середній досвід розробника становить 10 років, що свідчить про зрілий ринок.  
 - **Освіта:** Понад 43% фахівців використовують онлайн-курси як основне джерело знань, що підкреслює гнучкість сучасної ІТ-освіти.  
 - **Високооплачувані галузі:** Найвищі зарплати для віддаленої роботи зосереджені в секторах розробки програмного забезпечення, фінтех та охорони здоров'я.  

 ## Візуалізації  
Проєкт включає:  
 - **Гістограми розподілу досвіду.**
  
![Experience Distribution](https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/raw/main/results/work_experience_dist.png)
  
 - **Порівняльні діаграми зарплат "Медіана проти середнього" за країнами.**
  
![salaries by country](https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/raw/main/results/python_median_vs_mean.png)
  
 - **Кільцева діаграма розподілу форматів роботи (віддалена/гібридна/очна).**
  
![Analysis image 1](https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/raw/main/results/remote_work_pie_chart.png)
  
- **Тенденції популярності Python за віком.**
  
![Analysis image 1](https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/raw/main/results/python_popularity_by_age.png)  
  
## Структура проекту

**Stack-overflow-software-developer-survey-analysis/** — project directory  
    ├── data/ — project data  
    │ ├── raw/ — raw data  
    │ └── processed/ — cleaned data  
    ├── notebooks/ — main file with analysis code  
    ├── results/ — saved graphs and final tables  
    ├── reports/ — report of project  
    ├── requirements.txt — list of libraries to run the project  
    ├── .gitignore - git ignore patterns  
    ├── LICENSE — MIT License  
    ├── project-logo.png — project cover  
    └── README.md — project description  
  
## How to Use  
  
**How to use this project**  
To run this analysis locally, follow these steps:  
  
**1. Download the project file**  
  
[project-notebook.ipynb](https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/blob/main/notebooks/project-notebook.ipynb)  
  
File location: https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/blob/main/notebooks/
  
**2. Download the dataset**
  
[stack-overflow-developer-survey-2025.zip](https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/blob/main/data/raw/stack-overflow-developer-survey-2025.zip)  

File location:  
https://github.com/isachenko-andrii/Stack-overflow-software-developer-survey-analysis/blob/main/data/raw/ 

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
• **For Colab:** simply upload the project-notebook.ipynb file to your Google Drive.  
  
To connect the dataset to the project locally in step 1. "Data acquisition" of the project, replace the path to the **survey_results_schema.csv** and **survey_results_public.csv** files with the current one  
    
**Was:**  
srs_df_url = '/content/drive/MyDrive/ISAO/data/survey_results_schema.csv'  
srp_df_url = '/content/drive/MyDrive/ISAO/data/survey_results_public.csv'  
  
**Now:**   
srs_df_url = 'path to file /survey_results_schema.csv'  
srp_df_url = 'path to file /survey_results_public.csv'  
  
## Contact  
    
**Name:** [Andrii Isachenko](https://isachenko-andrii.github.io)    
**LinkedIn:** [Andrii Isachenko](https://www.linkedin.com/in/isachenko-andrii/)  
**E-mail:** isao.datastudio@gmail.com   
  
## Acknowledgments    
 
 - Thanks to the [Stack Overflow](https://survey.stackoverflow.co/) community for the open data.  
 - Thanks to the [Data Analyst/GoIT](https://goit.global/ua/courses/data-analytics/) course, which was part of this project.

---
  
**Project Status:** Completed. In the future, we plan to add analysis of the correlation between the use of AI tools and income level. Anomaly analysis - conducting a detailed study of the outliers segment.  
    
**License:** MIT License.  
