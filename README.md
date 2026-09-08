# Job Postings in AI-Related Field

## 🔎 Overview

Humanity is at a point where we almost step foot on a new era: Industry 5.0. This is a paradigm that sees humanity working side-to-side with advanced technology and AI-powered tools instead of being replaced by one.

> ⓘ Fully replacing physical labor with AI proves to be more costly, hence, the reason why this paradigm arose in the first place.

Two sentences above alone are able to shine a light on a conclusion: **In the future, only those who can make use of advanced technology and AI well enough will survive**

> ⓘ There are some exceptions of course of which the conclusion above do not apply (there are some jobs that are irreplacable by AI and further require human touch, e.g. Data Analyst).

Taking root in the conclusion, I decide to gather datasets that provide necessary data to prepare for war in job market and process them into actionable insights. The result will be in the form of interactive dashboard.
Download the database [here](https://www.kaggle.com/datasets/mann14/global-ai-and-data-science-job-market-20202026)

## 🛠 Tools I Use

1️⃣ Microsoft Excel ➜ Main tools to clean, process, and visualize data </br>
2️⃣ Visual Studio Code ➜ Place to write the README.md </br>
3️⃣ GitHub ➜ Version control </br>

## ✍ Data Preparation

1️⃣ Open a new workbook </br>
2️⃣ Open Power Query and load all the tables (except data_dictionary.csv) </br>
3️⃣ Make sure the data is clean for processing (search for blank, null, and error values) </br>
4️⃣ Open PowerPivot and create relationship between ai_jobs.csv and skills_demand.csv based on job_id

## ❓ Questions

1. Which jobs pay more or need more skills for each country?
2. Each country: median salary, top job type, and top skill throughout the year

## 📊📉 Analysis Approach

### 1. Job Title and Country Segmentation

Construct a pivot table with 3 columns
1. Job Title ➜ 6 job titles
2. Median Salary per Job Title ➜ Created using DAX Measurement
3. Skills per Job ➜ Created using DAX Measurement by dividing skills count and job count for each job

<img src="gifs\question_1.gif"
width = 100%>

> ⓘ Click the GIF to play it

#### 🗝️ Key Findings
- All 6 countries have the same order of job titles of highest median to lowest median
- All skills per job have similar value ranging between 4.4 and 4.5

#### 💡 Insight
The data does not reflect the real-world situation because they are to "ideal" and possess similar value to each other.

### 2. Mini Dashboard for Country and Year

<img src="gifs\question_2.gif"
width = 100%>

> ⓘ Click the GIF to play it

#### 🗝️ Key Finding
Each country and each year has its own trending job type, skill that appear the most in job postings, and job title order.

#### 💡 Insight
It is more likely that each country has its own deciding factors on job type, skill requirements, and job title rather than following fixed or seasonal trends.

## 🎓 What I Learned

1. Using Power Pivot to create relationship between two tables and merge two tables
2. Using DAX Measurement to create calculated formula and Power Pivot to create calculated column
3. Utilizing pivot table and multiple formula (XLOOKUP, SORT, UNIQUE, etc) to create the dashboard

## 🎯 Conclusions
1. Each country has its own most needed skills and top paid-jobs throughout the year
2. This dataset is too ideal and does not reflect real-world situation