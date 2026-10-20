<h1 align="center">📊 Data Analyst Job Market Analysis</h1> <p align="center"> <b>Which skills are most in demand, how are they trending, and which ones pay the most?</b><br> An end-to-end exploratory analysis of data job postings using Python. </p> <p align="center"> <img src="https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white" alt="Python"> <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white" alt="Pandas"><img src="https://img.shields.io/badge/Seaborn-Visualization-4C72B0" alt="Seaborn"> <img src="https://img.shields.io/badge/Matplotlib-Charts-11557C" alt="Matplotlib"> <img src="https://img.shields.io/badge/Jupyter-Notebooks-F37626?logo=jupyter&logoColor=white" alt="Jupyter"> </p>

📑 Table of Contents
<ol><li><a href="#-overview">Overview</a><br></li> <li><a href="#-the-questions">The Questions</a><br></li> <li><a href="#%EF%B8%8F-tools-i-used">Tools I Used</a><br></li><li><a href="#-project-structure">Project Structure</a><br></li> <li><a href="#-data-preparation-and-cleanup">Data Preparation and Cleanup</a><br></li> <li><a href="#-the-analysis">The Analysis</a><br></li> <li><a href="#-what-i-learned">What I Learned</a><br></li> <li><a href="#-challenges-i-faced">Challenges I Faced</a><br></li> <li><a href="#%EF%B8%8F-how-to-run-this-project">How to Run This Project</a><br></li> <li><a href="#-conclusion">Conclusion</a></li> </ol>

<h1>🔎 Overview</h1>

<h3>Welcome to my analysis of the data job market, focusing on data analyst roles.</h3>

<p>
This project was created out of a desire to navigate and understand the job market more effectively.
It delves into the <b>top-paying</b> and <b>in-demand</b> skills to help find optimal job opportunities for data analysts.
</p>

<h2>📦 About the Data</h2>

<p>
The data comes from a public data jobs dataset. It contains detailed information on job titles, salaries, locations, and essential skills.
Through a series of Python notebooks, I explore key questions such as the most demanded skills, skill trends over time, salary levels, and the intersection of demand and salary in data analytics.
</p>

<details>
  <summary><b>👉 Click to see what the dataset includes</b></summary>
  <br>
  <ul>
    <li><b>Job titles</b></li>
    <li><b>Salaries</b></li>
    <li><b>Locations</b></li>
    <li><b>Required skills</b></li>
  </ul>
</details>

<details>
  <summary><b>👉 Click to see what I explore</b></summary>
  <br>
  <ol>
    <li>The most demanded skills</li>
    <li>Skill trends over time</li>
    <li>Salary levels</li>
    <li>The intersection of demand and salary</li>
  </ol>
</details> 
<BR>

<h1>❓ The Questions</h1>

<h3>Below are the questions I wanted to answer in this project:</h3>

<ol>
  <li><b>What are the skills most in demand for the top 3 most popular data roles?</b></li>
  <br>
  <li><b>How are in-demand skills trending for Data Analysts?</b></li>
  <br>
  <li><b>How well do jobs and skills pay for Data Analysts?</b></li>
  <br>
  <li><b>What are the optimal skills for Data Analysts to learn?</b> (High Demand AND High Paying)</li>
</ol>

<details>
  <summary><b>👉 Click to see how I answer each question</b></summary>
  <br>
  <ol>
    <li>
      <b>Skill demand by role:</b> I count how often each skill appears in the postings for the top 3 roles and show the top 5 skills for each.<br>
      📓 Notebook: <code>2_Skill_Demand.ipynb</code>
    </li>
    <br>
    <li>
      <b>Skill trends:</b> I group Data Analyst skills by posting month to see how demand changes through the year.<br>
      📓 Notebook: <code>3_Skills_Trend.ipynb</code>
    </li>
    <br>
    <li>

<h1>🛠️ Tools I Used</h1>

<h3>For my deep dive into the data analyst job market, I used these key tools:</h3>

<table align="center">
  <thead>
    <tr>
      <th align="left">Tool</th>
      <th align="left">Purpose</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b>🐍 Python</b></td>
      <td>Backbone of the analysis</td>
    </tr>
    <tr>
      <td><b>🐼 Pandas</b></td>
      <td>Data cleaning, filtering, grouping, and aggregation</td>
    </tr>
    <tr>
      <td><b>📉 Matplotlib</b></td>
      <td>Base charts and formatting</td>
    </tr>
    <tr>
      <td><b>📊 Seaborn</b></td>
      <td>Advanced, cleaner statistical visuals</td>
    </tr>
    <tr>
      <td><b>🏷️ adjustText</b></td>
      <td>Non-overlapping labels on scatter plots</td>
    </tr>
    <tr>
      <td><b>📓 Jupyter / Google Colab</b></td>
      <td>Running code with notes and visual output side by side</td>
    </tr>
    <tr>
      <td><b>💻 Visual Studio Code</b></td>
      <td>Code editing and local execution</td>
    </tr>
    <tr>
      <td><b>🔀 Git &amp; GitHub</b></td>
      <td>Version control and sharing the project</td>
    </tr>
  </tbody>
</table>

<details>
  <summary><b>👉 Click to see the Python libraries I used</b></summary>
  <br>
  <ol>
    <li><b>Pandas:</b> analyze and reshape the data</li>
    <br>
    <li><b>Matplotlib:</b> build the base charts</li>
    <br>
    <li><b>Seaborn:</b> create more advanced visuals</li>
    <br>
    <li><b>adjustText:</b> keep scatter plot labels from overlapping</li>
  </ol>
</details>

<h3>🧹 Data Preparation and Cleanup</h3>

<p>This section outlines the steps taken to prepare the data for analysis, ensuring accuracy and usability.</p>

<h3>📥 Import &amp; Clean Up Data</h3>

<p>
I start by importing the necessary libraries and loading the dataset, then run initial cleaning tasks:
</p>

<ol>
  <li>Convert <code>job_posted_date</code> into a proper <b>datetime</b> type.</li>
  <br>
  <li>Convert the <code>job_skills</code> column from a string into a real <b>Python list</b> using <code>ast.literal_eval</code>.</li>
</ol>

<details>
  <summary><b>👉 Click to see the code</b></summary>
  <br>
<pre><code class="language-python"># Importing Libraries
import ast
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Loading Data
df = pd.read_csv('data_jobs.csv')

# Data Cleanup
df['job_posted_date'] = pd.to_datetime(df['job_posted_date'])
df['job_skills'] = df['job_skills'].apply(lambda x: ast.literal_eval(x) if pd.notna(x) else x)
</code></pre>
</details>

# Importing Libraries
import ast
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Loading Data
df = pd.read_csv('data_jobs.csv')

# Data Cleanup
df['job_posted_date'] = pd.to_datetime(df['job_posted_date'])
df['job_skills'] = df['job_skills'].apply(lambda x: ast.literal_eval(x) if pd.notna(x) else x)

Filter by Country

To focus the analysis on a single job market, I filter the dataset by country. Notebooks 2, 3 and 5 use India. Notebook 4 (salary analysis) uses the United States, because that is where most postings include salary data.

python
df_India = df[df['job_country'] == 'India']
df_US    = df[df['job_country'] == 'United States']
📈 The Analysis

Each Jupyter notebook in this project investigates a specific aspect of the data job market. Here is how I approached each question.

0️⃣ Exploratory Data Analysis

📓 Notebook: 1_EDA_Intro

Before answering the main questions, I explored the dataset to see what it contains:

Number of jobs per job title
Number of jobs per country (top 20)
Number of jobs per company (top 20)
Job benefits: work from home, degree requirement, and health insurance (pie charts)
Data Analyst jobs in India: top 10 job locations and benefit breakdown
Results
<p align="center"> <img src="images/Number_of_Jobs_per_Job_Title.png" width="700" alt="Number of Jobs per Job Title"> </p> <p align="center"><i>Bar chart showing how many postings exist for each data job title.</i></p> <p align="center"> <img src="images/Number_of_Jobs_per_Country.png" width="700" alt="Number of Jobs per Country"> </p> <p align="center"><i>Bar chart showing the 20 countries with the most postings.</i></p> <p align="center"> <img src="images/Job_Benefits_Pie_Charts.png" width="800" alt="Job Benefits"> </p> <p align="center"><i>Pie charts showing work-from-home, degree requirement, and health insurance shares.</i></p>
1️⃣ What are the most demanded skills for the top 3 most popular data roles?

📓 Notebook: 2_Skill_Demand

Approach:

Filter jobs by country.
Use explode() to turn each job's list of skills into one row per skill.
Count how often each skill appears per job title.
Convert counts to percentages by dividing by the total number of postings for that role. This makes the roles comparable.
Plot the top 5 skills for each of the top 3 roles.
Visualize Data
python
fig, ax = plt.subplots(len(job_titles), 1)

for i, job_title in enumerate(job_titles):
    df_plot = df_skills_perc[df_skills_perc['job_title_short'] == job_title].head(5)
    sns.barplot(data=df_plot, x='skill_percent', y='job_skills', ax=ax[i],
                hue='skill_count', palette='dark:b_r')

plt.show()
Results
<p align="center"> <img src="images/Likelihood_of_Skills_Requested_in_Job_Postings.png" width="750" alt="Likelihood of Skills Requested in Job Postings"> </p> <p align="center"><i>Bar graphs showing the top 5 skills (as a % of postings) for each of the top 3 data roles.</i></p>
💡 Insights
📝 Which skill is the most requested for each role? Write the skill and its percentage from your chart.
📝 How do the skills differ between roles (for example analyst tools vs. engineering tools)?
📝 Which skill appears across all three roles?
2️⃣ How are in-demand skills trending for Data Analysts?

📓 Notebook: 3_Skills_Trend

Approach:

Filter Data Analyst postings.
Extract the posting month with dt.month.
Pivot the data so each row is a month and each column is a skill.
Divide by the monthly total of postings to get the likelihood of a skill in a posting.
Plot the top 5 skills as lines across the months of 2023.
Visualize Data
python
from matplotlib.ticker import PercentFormatter

df_plot = df_DA_India_percent.iloc[:, :5]
sns.lineplot(data=df_plot, dashes=False, legend='full', palette='tab10')

plt.gca().yaxis.set_major_formatter(PercentFormatter(decimals=0))
plt.show()
Results
<p align="center"> <img src="images/Trending_Top_Skills_for_Data_Analysts.png" width="750" alt="Trending Top Skills for Data Analysts"> </p> <p align="center"><i>Line chart showing the monthly likelihood of the top 5 skills in Data Analyst postings in 2023.</i></p>
💡 Insights
📝 Which skill stays the most consistent through the year?
📝 Which skill rises or falls the most?
📝 Note any months with missing or sparse data, since small samples make the lines noisy.
3️⃣ How well do jobs and skills pay for Data Analysts?

📓 Notebook: 4_Salary_Analysis

I used only jobs that include salary_year_avg and compared the median salary (the median is less affected by extreme outliers than the mean).

3a. Salary distribution by job title

I took the 6 most common job titles and compared their salary distributions with a box plot, ordered by median salary.

python
sns.boxplot(data=df_US_top6, x='salary_year_avg', y='job_title_short', order=job_order)

ticks_x = plt.FuncFormatter(lambda y, pos: f'${int(y/1000)}K')
plt.gca().xaxis.set_major_formatter(ticks_x)
plt.show()
<p align="center"> <img src="images/Salary_Distributions_of_Data_Jobs_in_the_US.png" width="750" alt="Salary Distributions of Data Jobs in the US"> </p> <p align="center"><i>Box plot showing the salary distributions for the top 6 data job titles.</i></p>
3b. Highest-paid vs. most in-demand skills for Data Analysts

I then focused on Data Analyst roles only and built two bar charts: one for the 10 highest-paid skills and one for the 10 most in-demand skills (with their median salary).

python
fig, ax = plt.subplots(2, 1)

# Top 10 highest paid skills
sns.barplot(data=df_DA_top_pay, x='median', y=df_DA_top_pay.index,
            hue='median', ax=ax[0], palette='dark:b_r')

# Top 10 most in-demand skills
sns.barplot(data=df_DA_skills, x='median', y=df_DA_skills.index,
            hue='median', ax=ax[1], palette='light:b')

plt.show()
<p align="center"> <img src="images/Highest_Paid_and_Most_In_Demand_Skills_for_Data_Analysts.png" width="750" alt="Highest Paid and Most In-Demand Skills for Data Analysts"> </p> <p align="center"><i>Top: highest-paid skills. Bottom: most in-demand skills, both by median salary.</i></p>
💡 Insights
📝 Which job title has the highest median salary, and which has the widest spread?
📝 Which roles show many high-end outliers?
📝 Which skills pay the most? Check each skill's count first, because a high median based on very few postings is not reliable.
📝 How do the highest-paid skills differ from the most in-demand skills?
4️⃣ What are the most optimal skills to learn for Data Analysts?

📓 Notebook: 5_Optimal_skills

The optimal skills are the ones that are both high demand and high paying.

Approach:

Count how many Data Analyst postings (with salary) mention each skill.
Compute skill_percent (share of postings) and median_salary for each skill.
Keep only skills present in more than 5% of postings.
Plot demand (x-axis) against median salary (y-axis). Skills in the top-right are the best ones to learn.
Visualize Data
python
from adjustText import adjust_text

plt.scatter(df_DA_skills_high_demand['skill_percent'],
            df_DA_skills_high_demand['median_salary'])
plt.show()
Results
<p align="center"> <img src="images/Most_Optimal_Skills_for_Data_Analysts.png" width="750" alt="Most Optimal Skills for Data Analysts"> </p> <p align="center"><i>Scatter plot of skill demand (% of postings) against median salary.</i></p>
🎨 Visualizing Different Technologies

I grouped skills into technology categories and colored the scatter plot by category:

Category	Skills
Programming	Python, R, SQL
Analyst tools	Excel, Tableau, Power BI, PowerPoint, Word, Visio
Cloud	AWS, Azure, GCP
Databases	SQL Server, MongoDB, Oracle, Redshift, MySQL, PostgreSQL
Other	Spark, Hadoop, Flow, Zoom, and others
python
sns.scatterplot(
    data=df_DA_skills_tech_high_demand,
    x='skill_percent',
    y='median_salary',
    hue='technology'
)
plt.show()
<p align="center"> <img src="images/Most_Optimal_Skills_for_Data_Analysts_by_Technology.png" width="750" alt="Most Optimal Skills colored by Technology"> </p> <p align="center"><i>Scatter plot of optimal skills, colored by technology category.</i></p>
💡 Insights
📝 Which skills sit in the top-right corner (high demand and high salary)?
📝 Which skills are very common but pay less?
📝 Which technology category clusters at the highest salaries?
🎓 What I Learned
Advanced Pandas: explode(), groupby(), pivot_table(), merge(), and percentage calculations.
Data cleaning matters: converting stringified lists and dates correctly is essential before any analysis.
Choosing the right chart: bar charts for rankings, line charts for trends, box plots for distributions, scatter plots for trade-offs.
Strategic skill analysis: demand and salary together say more than either one alone.
🧗 Challenges I Faced
Data inconsistencies: missing salary values and missing skill lists required careful filtering.
Small sample sizes: some months and skills have few postings, which makes percentages and medians noisy.
Complex visualization: keeping labels readable (for example with adjustText) and scales comparable across subplots.
Breadth vs. depth: deciding how deep to go on each question without losing the big picture.
▶️ How to Run This Project

1. Clone the repository

bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>

2. Install the requirements

bash
pip install pandas seaborn matplotlib adjustText jupyter

3. Add the dataset

Download the data from Luke Barousse's Python Course and place the CSV file in the project folder. Update the file path in the first cell of each notebook.

4. Run the notebooks in order

bash
jupyter notebook

5. Save your charts for this README

Add this line after each plt.show() so the images appear in the images/ folder:

python
plt.savefig('images/Your_Chart_Name.png', dpi=200, bbox_inches='tight')
✅ Conclusion

This exploration of the data analyst job market highlights the skills and trends that shape the field. By combining demand (how often a skill is requested) with pay (the median salary), the analysis points to the skills that give the best return on learning time. Job markets change quickly, so re-running these notebooks on fresh data is a good way to keep the findings current.

<p align="center"> ⭐ If you found this project useful, please consider giving it a star! </p>