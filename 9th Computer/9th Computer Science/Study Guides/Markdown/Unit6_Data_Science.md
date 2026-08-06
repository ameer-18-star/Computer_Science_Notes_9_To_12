# Unit 6: Data Science and Data Gathering

---

> **"Without data, you're just another person with an opinion."**
> — W. Edwards Deming, statistician and engineer

---

## Student Learning Outcomes

By the end of this chapter, you will be able to:

- **Identify and differentiate** between qualitative and quantitative data, and explain their importance in analysis.
- **Organise data** effectively and apply basic data analysis techniques to draw meaningful conclusions.
- **Describe data collection methods and tools**, including surveys, questionnaires, and online sources.
- **Explain data storage techniques** — spreadsheets, databases, and cloud storage — and understand their uses.
- **Apply data pre-processing techniques** to clean and prepare data for analysis.
- **Use data visualization tools** to represent data through charts and graphs.
- **Understand cloud storage and collaborative tools** and apply best practices for data protection.
- **Be aware of ethical practices** related to data privacy, confidentiality, and secure data handling.
- **Explain the concept of data science**, its scope, and its impact on real-world applications.
- **Describe big data** and its applications in healthcare, finance, retail, and transportation.
- **Know key data science tools** including Excel, Python, R, and SQL.

---

## Introduction

Every single day, you produce data — and you do not even realize it.

When you check your phone in the morning, the app records when you woke up. When you search for a song on YouTube, the platform records what you searched for. When you buy a snack from the school canteen, the cashier records the sale.

All of this — your habits, your choices, your movements — is **data**.

Data is everywhere. And the people who know how to collect it, organize it, clean it, and understand it have one of the most powerful skills of the 21st century.

In this chapter, you will learn to think like a **data scientist**. You will learn what data is, how to collect it, how to clean it, how to visualize it, and how to draw useful conclusions from it. You will discover tools used by professionals — from Google Sheets to Python — and understand why "messy data" is not a failure; it is just a problem waiting to be solved.

Let's become detectives of data.

---

## 6.1 Data

### What Is Data?

---

#### 🔖 The Hook

In 1854, London was struck by a deadly cholera outbreak. People were dying every day, and no one knew why. A doctor named **John Snow** — not the one from Game of Thrones — had an idea. Instead of guessing, he went street by street and **collected data**: he recorded the name, address, and date of death of every cholera victim.

Then he plotted each death on a map of London.

The pattern was clear: almost all deaths clustered around a single water pump on Broad Street. Snow removed the pump handle. The outbreak stopped almost immediately.

John Snow did not find the answer through luck or guessing. He found it through **data**.

---

#### 📖 The Explanation

> **Definition:** Data consists of raw facts collected about things around us that we can process to generate useful information.

The key word is **raw**. Data on its own does not tell you much. It is just facts — numbers, words, measurements, observations, images, sounds. When you **process** data — organize it, analyze it, look for patterns — it becomes **information** that you can act on.

**Data can take many forms:**

| Form of Data | Example |
|-------------|---------|
| **Numbers** | Test scores: 85, 78, 92 |
| **Words** | Student names: Ali, Sara, Ahmed |
| **Measurements** | Temperature: 37°C |
| **Observations** | "The student was absent on Monday." |
| **Images** | A photo taken on a smartphone |
| **Sounds** | A voice recording |

**Data can come from many sources:**
- Surveys and questionnaires
- Sensors and smartwatches
- Social media posts
- Hospital records
- Weather stations
- School attendance registers

---

#### ✋ Interactive Stop-Point: Pause & Think

Think about yesterday. List **five pieces of data** that were collected about you — even without you knowing. Think about your phone, your school, your home, and any apps you used.

*(Example: "My phone recorded how many steps I walked.")*

How many of those pieces of data do you think are being used by someone right now?

---

#### 📌 Quick Recap

> **Data is raw facts — numbers, words, measurements, images — collected from the world around us. On its own it means little; processed, it becomes powerful information.**

---

## 6.2 Data Types

### How Is Data Classified?

Data is divided into two broad categories: **Qualitative** and **Quantitative**. Understanding the difference is the first step toward analyzing any data correctly.

---

### 6.2.1 Qualitative Data

---

#### 🔖 The Hook

Your teacher asks the class: "What is your favourite school subject?" Students answer: "Computer Science." "Mathematics." "Art." "Physics."

Can you add these answers together? Can you calculate an average? No — you cannot add "Art" and "Physics" together. These are descriptions, not numbers.

That is qualitative data.

---

#### 📖 The Explanation

> **Definition:** Qualitative data refers to categories or labels that describe the **qualities or characteristics** of something — not the quantity. It answers the question: *"What kind?"* or *"What type?"*

Qualitative data is always described in **words, labels, or symbols** — never in numbers.

**Key characteristics of qualitative data:**

| Characteristic | Explanation | Example |
|---------------|-------------|---------|
| **Non-Numeric** | Represented by words or labels, not numbers. | Names of students: Ali, Sara, Ahmed |
| **Categorical** | Can be divided into groups or categories. | Types of fruit: apple, mango, banana |
| **Descriptive** | Describes attributes, qualities, or characteristics. | Colours: red, blue, green |

**More examples of qualitative data:**
- The name of your city (Lahore, Karachi, Islamabad)
- Your blood group (A, B, AB, O)
- The genre of a book (fiction, non-fiction, science)
- A student's feedback: "The lesson was very interesting."
- The colour of a car

---

#### ✋ Interactive Stop-Point: Grab a Partner

Look at this list of data and identify which items are qualitative:

1. The temperature today: 35°C
2. Your favourite colour: Blue
3. The number of students in your class: 32
4. The type of mobile phone you use: Android
5. Your height: 165 cm
6. The language you speak at home: Urdu

Which are qualitative? Write them down and explain why.

---

#### 📌 Quick Recap

> **Qualitative data describes qualities in words — it cannot be measured with a ruler or calculated with a formula. It answers "what kind?" not "how many?"**

---

### 6.2.2 Quantitative Data

---

#### 🔖 The Hook

Your school wants to compare the performance of two classes. Class A has an average score of 78. Class B has an average score of 85. You can immediately see that Class B performed better.

Why? Because you are working with **numbers** — and numbers can be compared, added, subtracted, and averaged. That is quantitative data doing its job.

---

#### 📖 The Explanation

> **Definition:** Quantitative data consists of numbers used to **measure the quantity or amount** of something. It answers the questions: *"How many?"* or *"How much?"* or *"How long?"*

Quantitative data can be used in mathematical calculations and statistical analyses.

**Key characteristics of quantitative data:**

| Characteristic | Explanation | Example |
|---------------|-------------|---------|
| **Numerical** | Expressed in numbers. | Heights: 160 cm, 172 cm, 158 cm |
| **Measurable** | Can be measured using tools. | Temperature measured with a thermometer |
| **Countable** | Can be counted. | Number of students: 32 |
| **Arithmetical** | Can be used in calculations. | Monthly fee × 12 = Annual fee |

**More examples of quantitative data:**
- A student's test score: 85 out of 100
- The weight of a bag: 4.5 kg
- The number of pages in a book: 320
- The time taken to run 100 metres: 13.4 seconds
- The price of a notebook: Rs. 50

---

#### 📝 Comparing Qualitative vs. Quantitative Data

| Feature | Qualitative | Quantitative |
|---------|------------|--------------|
| **Represents** | Descriptions and categories | Numbers and amounts |
| **Answers** | "What kind?" "What type?" | "How many?" "How much?" |
| **Example** | Favourite colour: Blue | Age: 14 years |
| **Can be calculated?** | No | Yes |
| **Can be graphed?** | As categories | As numbers on a scale |

---

#### ✋ Interactive Stop-Point: Pause & Think

A school is doing a survey of its students. Classify each piece of data below as either **qualitative** or **quantitative**:

1. The number of books a student reads per month.
2. A student's favourite sport.
3. The distance from home to school (in km).
4. The country a student was born in.
5. A student's score on the last maths test.
6. The colour of a student's school bag.
7. The number of siblings a student has.
8. A student's opinion on school uniform: "I like it" or "I don't like it."

Compare your answers with your partner. Did you agree on all eight?

---

#### 📌 Quick Recap

> **Quantitative data uses numbers to measure and count. It can be calculated, compared, and graphed on a number scale. It answers "how many?" and "how much?"**

---

## 6.3 Organising and Analysing Data

### Why Organisation Matters

---

#### 🔖 The Hook

Imagine your teacher keeps all student records on loose sheets of paper scattered across her desk. When she needs to find your attendance record, she has to search through 200 sheets. It takes 20 minutes.

Now imagine the same records in a tidy table — student names in one column, attendance in another, dates across the top. Finding your record takes 10 seconds.

The data is exactly the same. The difference is **organisation**.

---

#### 📖 The Explanation

> **Definition:** Organising data means arranging raw facts into a structured format — such as a table, chart, or graph — that makes it easier to read, compare, and analyze.

**Why is organising data important?**

| Benefit | Explanation |
|---------|-------------|
| **Saves time** | Finding specific information is faster in organized data. |
| **Reduces errors** | Neat tables prevent mistakes like recording a score under the wrong name. |
| **Improves clarity** | Organized data is easier to read and understand. |
| **Enables decisions** | Patterns and conclusions become visible when data is well arranged. |

---

#### 📝 Three Ways to Organise Data

**Method 1: Data Tables**

A table organizes data into rows and columns. Each row is one record. Each column is one attribute (type of information).

**Example: Student Scores Table**

| Student | Maths | Science | English |
|---------|-------|---------|---------|
| Ali | 85 | 78 | 90 |
| Sara | 78 | 88 | 85 |
| Ahmed | 92 | 82 | 87 |
| Fatima | 90 | 80 | 89 |
| Bilal | 67 | 75 | 70 |

At a glance, you can see who scored highest in Maths (Ahmed: 92) and who needs support in all subjects (Bilal).

---

**Method 2: Charts**

A chart is a visual representation of data. It turns numbers into pictures, making patterns obvious at a glance.

**Common types of charts:**

| Chart Type | Best Used For | Example |
|-----------|--------------|---------|
| **Bar Chart** | Comparing different categories | Comparing scores of 5 students |
| **Pie Chart** | Showing parts of a whole | Showing % of students who like each subject |
| **Line Chart** | Showing change over time | Showing a student's score trends over 6 months |

**How to describe a bar chart on paper:**

Draw a horizontal axis (x-axis) and a vertical axis (y-axis). Label the x-axis with student names (Ali, Sara, Ahmed, Fatima, Bilal). Label the y-axis with scores from 0 to 100. Draw a vertical bar for each student reaching up to their Maths score. Title the chart: "Maths Scores of Students."

---

**Method 3: Graphs**

A graph is similar to a chart but often shows the **relationship** between two sets of data.

**Common types of graphs:**

| Graph Type | Best Used For |
|-----------|--------------|
| **Line Graph** | Showing trends and changes over time |
| **Bar Graph** | Comparing quantities across categories |
| **Scatter Plot** | Showing the relationship between two variables |
| **Histogram** | Showing how often data falls into ranges |

**Example: A line graph** showing Ali's test scores over six months would have months on the x-axis and scores on the y-axis. A rising line means improvement. A falling line means decline.

---

### Methods and Tools of Data Collection

> **Definition:** Data collection is the process of **gathering information** to answer questions, make decisions, or understand something better.

Before you can organize or analyze data, you must collect it. Here are the main methods:

---

#### 📖 Method 1: Surveys

> **Definition:** A survey collects information from a group of people by asking them standardized questions.

Surveys can be done on paper, by phone, or online.

**Example:** You want to know your classmates' favourite ice cream flavours. You create a survey with the question: *"What is your favourite ice cream flavour? (Chocolate / Vanilla / Strawberry / Other)"* and give it to your whole class.

**Best practices for designing a good survey:**
- Keep questions **short and specific**.
- Use **multiple choice** or **rating scales** where possible (e.g., "Rate from 1 to 5").
- Avoid leading questions. (Do NOT say: "Don't you agree that...?")
- Ensure **anonymity** — people answer more honestly when they are not identified.
- **Test your survey** with two or three people before distributing it widely.

**Online survey tools:**
- **Google Forms** — free, easy to use. Visit: https://forms.google.com
- **Microsoft Forms** — similar to Google Forms. Visit: https://forms.office.com
- **SurveyMonkey** — professional survey platform. Visit: https://www.surveymonkey.com

---

#### 📖 Method 2: Questionnaires

> **Definition:** A questionnaire is a written form with a set of questions for people to fill out — similar to a survey but usually more structured and formal.

**Example:** Your school wants to know which extracurricular activities students enjoy most. They distribute a questionnaire with the question: *"Which school activity do you enjoy most? (Sports / Art / Music / Drama)"*

The difference between a survey and a questionnaire is subtle: surveys are often broader and can be verbal or digital, while questionnaires are typically written documents with fixed questions.

---

#### 📖 Method 3: Interviews

> **Definition:** An interview involves talking to a person one-on-one to gather detailed, in-depth information.

**Example:** Your school wants to understand why some teachers find online classes difficult. They interview five teachers individually, asking open questions like: *"What challenges do you face when teaching online?"*

Interviews are better for **qualitative data** — they capture opinions, experiences, and feelings that a simple survey cannot.

---

#### 📖 Method 4: Observations

> **Definition:** Observation involves watching a situation and noting what happens — without asking anyone questions.

**Example:** A teacher watches students during a group project to observe who participates actively, who stays quiet, and how decisions are made. She records her observations in a notebook.

Observation is especially useful when people's **behavior** is more informative than their **words**.

---

#### 📖 Method 5: Online Data Sources

> **Definition:** Online data sources are websites, digital databases, and online tools where data has already been collected and is available for use.

**Examples:**
- Government websites with population statistics.
- Weather websites with historical temperature data.
- World Bank or UN databases with global health and education data.
- Wikipedia for general factual information.

Online sources save time — the data is already collected. But you must **verify the source** is trustworthy.

---

#### 🏫 Class Activity: Collect Your Own Data

**Step 1:** Choose a topic. Example: "Which sport is most popular in our class?"

**Step 2:** Design a short survey with 3–5 clear questions. Use multiple choice options.

**Step 3:** Share the survey with your classmates and collect responses.

**Step 4:** Enter the responses into a table (on paper or in a spreadsheet).

**Step 5:** Create one chart from the data — a bar chart or pie chart works well for this type of question.

**Step 6:** Present your chart to the class and explain what the data shows.

---

#### ✋ Interactive Stop-Point: Pause & Think

You want to find out why students at your school are coming late in the morning.

1. Which data collection method would you use: survey, interview, observation, or online sources? Why?
2. Write three questions you would ask.
3. Would the data you collect be qualitative, quantitative, or both?

---

#### 📌 Quick Recap

> **Organising data into tables, charts, and graphs makes patterns visible and analysis easier. Data can be collected through surveys, questionnaires, interviews, observations, or online sources — each method has its own strengths.**

---

## 6.4 Data Types and Formats

### Structured vs. Unstructured Data

When data is stored and processed by computers, it takes two main formats: **structured** and **unstructured**.

---

### 6.4.1 Structured Data

---

#### 🔖 The Hook

Think of a school database. Every student has a number, a name, a class, a date of birth, a fee status, and a height. All this information is stored neatly in rows and columns — like a very organized spreadsheet.

When the admin needs to find all students in Class 9 who have not paid their fees, the system can answer that question in seconds. Why? Because the data is **structured**.

---

#### 📖 The Explanation

> **Definition:** Structured data is data that is **organised and formatted** in a fixed, predefined way that makes it easy to search and analyze.

Structured data lives in rows and columns — in spreadsheets, tables, and databases. Each column has a specific type of information. Each row is one record.

**Example: Structured Student Database**

| Student # | Student Name | Class | Date of Birth | Fee Status | Height |
|-----------|-------------|-------|--------------|------------|--------|
| 001 | Ali Akbar | 9th | 25/03/2009 | Paid | 4.7 ft |
| 002 | Faheem Aslam | 9th | 07/05/2008 | Paid | 4.9 ft |
| 003 | Munir Ahmad | 9th | 11/06/2009 | Unpaid | 5.2 ft |
| 004 | Khalid Mahmood | 9th | 13/09/2009 | Paid | 5.6 ft |
| 005 | Kamran Malik | 9th | 21/07/2009 | Paid | 5.3 ft |

**Why structured data is powerful:**
- Easy to search: "Show me all students who have NOT paid fees."
- Easy to sort: "Sort students by height."
- Easy to calculate: "Calculate the average height."
- Easy to filter: "Show only students born in 2009."

**Where is structured data used?**
- School databases (student records)
- Bank account systems (transactions)
- Hospital patient records
- E-commerce order systems (products, prices, quantities)

---

#### ✋ Interactive Stop-Point: Pause & Think

Your school wants to create a structured database for the school library. Every book needs to be recorded.

Design a table with **at least 5 column headers** that you would include. For example: Book Title, Author...

What other information would be useful to store? Why?

---

#### 📌 Quick Recap

> **Structured data is neatly organised in rows and columns — easy to search, sort, filter, and calculate. It is the format used in spreadsheets and databases.**

---

### 6.4.2 Unstructured Data

---

#### 🔖 The Hook

You open Instagram and scroll through your feed. You see a photo of a friend's birthday cake. A funny video of a cat. A news article someone shared. A voice note someone posted. Comments like "So cute! 😍" and "WOW!!!"

Can you put all of that into a neat table with rows and columns?

No — because it is **unstructured data**.

---

#### 📖 The Explanation

> **Definition:** Unstructured data is data that **does not fit into a fixed format**. It is free-form and cannot be neatly organized into rows and columns.

Unstructured data is the **majority of data** produced in the world today. Emails, social media posts, photos, videos, audio recordings, PDF documents, and chat messages are all examples.

**Examples of unstructured data:**

| Type | Example |
|------|---------|
| **Text** | An email, a WhatsApp message, a blog post |
| **Social media posts** | A tweet, an Instagram caption, a Facebook update |
| **Images** | A photo, a medical X-ray, a scanned document |
| **Videos** | A YouTube video, a CCTV recording |
| **Audio** | A voice recording, a podcast, a phone call |

**The challenge of unstructured data:**

Unstructured data is harder to analyze because computers cannot simply search a column for a value. Special tools — like AI, machine learning, and natural language processing — are needed to extract meaning from unstructured data.

For example, to analyze 10,000 customer reviews (text) and find out whether customers are happy or unhappy, you need sophisticated tools — not just a filter button on a spreadsheet.

---

#### 📝 Structured vs. Unstructured — Side by Side

| Feature | Structured Data | Unstructured Data |
|---------|----------------|-------------------|
| **Format** | Fixed — rows and columns | Free-form — no fixed format |
| **Examples** | Spreadsheets, databases | Emails, videos, images, posts |
| **Easy to search?** | Yes — using filters and queries | No — needs special tools |
| **Storage** | Traditional databases | Cloud storage, data lakes |
| **Amount in the world** | Small minority | Vast majority (80%+) |

---

#### ✋ Interactive Stop-Point: Grab a Partner

Sort each item below into **Structured** or **Unstructured**:

1. A school fee receipt in a spreadsheet.
2. A student's WhatsApp message to a teacher.
3. A database of book prices in a library.
4. A photo of a class on Sports Day.
5. A patient's medical history in a hospital database.
6. A doctor's handwritten notes about a patient.
7. A list of cricket scores in a table.
8. A YouTube video of a cricket match.

Discuss: Why do you think unstructured data is harder to analyze?

---

#### 📌 Quick Recap

> **Unstructured data has no fixed format — emails, photos, videos, and social media posts are examples. It makes up the vast majority of data in the world and requires special tools to analyze.**

---

## 6.5 Data Visualization

### Turning Numbers Into Pictures

---

#### 🔖 The Hook

In 1854, John Snow's map of cholera deaths (from our earlier story) was one of the first examples of **data visualization** in history. By plotting data on a map, he saw a pattern that no amount of reading numbers could have revealed.

Today, every time you see a weather forecast with colorful temperature maps, a cricket match with a score graph, or a COVID-19 case tracker — you are seeing data visualization at work.

A picture does not just tell a thousand words. Sometimes, it tells you something that a thousand numbers cannot.

---

#### 📖 The Explanation

> **Definition:** Data visualization is the process of turning numbers and data into visual representations — charts, graphs, and maps — that make it easier to understand patterns, trends, and relationships.

**Why is visualization important?**

- The human brain processes visual information **60,000 times faster** than text.
- Patterns and trends hidden in rows of numbers become **instantly obvious** in a chart.
- Visualizations make it easier to **communicate findings** to others — including people who are not data experts.

---

#### 📝 Types of Visualizations and When to Use Them

**1. Bar Chart**

**What it shows:** Comparison between different categories.

**When to use it:** When you want to compare quantities across different groups.

**Example:** Comparing the number of students who prefer each subject.

**How to draw it:**
- Draw an x-axis (horizontal) and a y-axis (vertical).
- Label the x-axis with your categories (Maths, Science, English, Urdu).
- Label the y-axis with numbers (0 to 40).
- Draw a vertical bar for each category reaching up to its value.
- Title: "Favourite Subject of Class 9 Students"

---

**2. Pie Chart**

**What it shows:** Parts of a whole — how a total is divided into portions.

**When to use it:** When you want to show percentages or proportions.

**Example:** 50% of students prefer Maths, 30% prefer Science, 20% prefer English.

**How to draw it:**
- Draw a circle.
- Divide it into slices. A 50% slice takes up half the circle. A 30% slice takes up slightly less than a third. A 20% slice takes up the remaining portion.
- Label each slice with the category and percentage.
- Title: "Subject Preferences in Class 9 (%)"

---

**3. Line Graph**

**What it shows:** Change over time — trends going up, down, or staying flat.

**When to use it:** When you want to track something over a period.

**Example:** A student's test score in Maths every month for 6 months.

**How to draw it:**
- Draw an x-axis (months: Jan, Feb, Mar...) and a y-axis (scores: 0 to 100).
- Plot a dot for each month at the correct score.
- Connect the dots with a line.
- A rising line = improvement. A falling line = decline.
- Title: "Ali's Maths Scores Over 6 Months"

---

**4. Scatter Plot**

**What it shows:** The relationship between two variables.

**When to use it:** When you want to see if two things are related.

**Example:** Is there a relationship between study hours and test scores?

**How to draw it:**
- X-axis: Hours studied per week.
- Y-axis: Test score.
- For each student, plot one dot at the intersection of their study hours and score.
- If dots trend upward (right), there is a positive relationship — more study = higher score.

---

### Data Visualization Tools

---

#### 📖 The Tools

| Tool | What It Is | Best For |
|------|-----------|---------|
| **Microsoft Excel** | Spreadsheet with built-in charting | Basic charts and graphs for students and professionals |
| **Google Sheets** | Online spreadsheet, free, shareable | Creating and sharing visualizations collaboratively |
| **Tableau** | Dedicated visualization software | Advanced, interactive, and professional visualizations |
| **Microsoft Power BI** | Business visualization platform | Creating dashboards with multiple chart types, maps, and more |

**For students:** Start with **Microsoft Excel** or **Google Sheets**. They are free, easy to learn, and powerful enough to create any chart type you will need in this course.

---

#### 📝 Step-by-Step: Create a Bar Chart in Google Sheets

**Step 1:** Open Google Sheets (sheets.google.com) and create a new spreadsheet.

**Step 2:** Enter your data in two columns:

```
Column A       Column B
Subject        Number of Students
Maths          15
Science        10
English        8
Urdu           7
```

**Step 3:** Select all the data (A1 to B5).

**Step 4:** Click **Insert** → **Chart**.

**Step 5:** In the Chart Editor panel, choose **Chart type: Bar chart** (or Column chart).

**Step 6:** Add a title: "Favourite Subject of Class 9 Students."

**Step 7:** Your bar chart appears. You can change colours, add labels, and download it as an image.

---

#### ✋ Interactive Stop-Point: Grab a Partner

You have the following data from a survey of 40 students about their favourite sport:

| Sport | Number of Students |
|-------|--------------------|
| Cricket | 18 |
| Football | 10 |
| Basketball | 7 |
| Badminton | 5 |

1. What type of chart would you use to show this data? Why?
2. Draw the chart by hand on paper. Label all axes and give the chart a title.
3. Now convert the numbers to percentages and draw a pie chart of the same data.
4. Which chart communicates the information more clearly? Discuss with your partner.

---

#### 📌 Quick Recap

> **Data visualization turns raw numbers into charts and graphs — bar charts for comparisons, pie charts for proportions, line graphs for trends over time. Tools like Excel and Google Sheets make this easy for beginners.**

---

## 6.6 Data Pre-Processing and Analysis

### Cleaning Data Before Using It

---

### 6.6.1 What Is Data Pre-Processing?

---

#### 🔖 The Hook

Imagine a chef about to cook a special meal. Before she can start cooking, she must wash the vegetables, remove the bad ones, peel them, and cut them to the right size. Only then can cooking begin.

If she skips this preparation and throws dirty, unpeeled vegetables into the pot — the meal will be terrible, no matter how good her cooking skills are.

**Data pre-processing is exactly this preparation step for data.**

---

#### 📖 The Explanation

> **Definition:** Data pre-processing is the process of **cleaning and organising raw data** to make it accurate, complete, and ready for analysis.

Raw data collected from the real world is almost never perfect. It can have:
- **Missing values** (someone forgot to fill in a field)
- **Errors** (a score of 105 out of 100)
- **Duplicates** (the same record entered twice)
- **Outliers** (values that are unusually high or low)
- **Inconsistencies** (one record says "Male", another says "M")

If you analyze dirty data, your conclusions will be wrong — even if your analysis is perfect. The saying in data science is: **"Garbage in, garbage out."**

---

### 6.6.2 Data Pre-Processing Techniques

---

#### 📖 Technique 1: Evaluating Data Quality

Before fixing anything, first **assess** the data. Ask these questions:

| Question | What You Are Checking |
|---------|----------------------|
| Is any data missing? | Are there empty cells or blank fields? |
| Are there errors? | Are any values impossible or incorrect? |
| Is the data consistent? | Do similar records use the same format? |
| Is the data current? | Is this data from the right time period? |

**Example:** You have a spreadsheet of student test scores. Before analysis, check:
- Does every student have a score recorded? (Missing data check)
- Are all scores between 0 and 100? (Error check)
- Are all dates in the same format — e.g., DD/MM/YYYY? (Consistency check)

---

#### 📖 Technique 2: Identifying Errors, Outliers, and Biases

**Errors** are mistakes in the data.

**Example:** If the maximum marks of a subject are 100 and a student's score is recorded as 105, that is clearly an error — scores cannot exceed 100.

**How to spot errors:** Check if values fall within a valid range. Set rules: "All scores must be between 0 and 100."

---

**Outliers** are unusual or extreme values that do not fit the pattern of the rest of the data.

**Example:** If most students scored between 60 and 85, but one student scored 5, the score of 5 is an outlier.

An outlier is not necessarily wrong — it might be a real value. But it must be **investigated** before you decide to keep or remove it.

**How to spot outliers:** Sort the data. Look at the highest and lowest values. Do they make sense?

---

**Biases** are distortions in the data that make it unrepresentative.

**Example:** If you survey only students from one school to understand the opinion of students across the whole city, your data is **biased** — it does not represent the full population.

**How to avoid bias:** Make sure your data collection covers a wide and diverse sample.

---

### 6.6.3 Implementing Data Validation and Cleaning

---

#### 📖 Step 1: Data Validation

> **Definition:** Data validation means checking the data to ensure it is **complete and accurate**.

**Validating completeness:** Make sure no data is missing.

**Example:** Check that every student in the list has a test score. If Student ID 003 has no score recorded, that is an incomplete record.

**Validating accuracy:** Make sure all values are correct and within the expected range.

**Example:** Verify that all test scores are between 0 and 100. Any value outside this range is invalid.

---

#### 📖 Step 2: Data Cleaning

> **Definition:** Data cleaning means **fixing or removing** errors, inconsistencies, and missing values so the data is ready for analysis.

**How to handle errors:**
- If you know the correct value, **fix it**. (Change 105 to the correct score.)
- If you do not know the correct value, **delete the record**. It is better to have less data than wrong data.

**How to handle missing data:**
- **Fill in** the missing value using a reasonable estimate. (Example: use the class average score to fill in a missing student score.)
- **Delete** the incomplete record if the missing field is critical.

**How to handle outliers:**
- **Investigate first.** Ask: Is this a real value or a mistake?
- If it is a mistake, correct or remove it.
- If it is a true value (e.g., a genuinely exceptional student), keep it — but note it in your analysis.

---

#### 📝 Step-by-Step: Cleaning a Dataset

You have this raw dataset of student scores:

| Student | Score |
|---------|-------|
| Ali | 85 |
| Sara | 105 |
| Ahmed | 78 |
| Fatima | (blank) |
| Bilal | 3 |

**Step 1 — Check for errors:** Sara's score of 105 exceeds the maximum of 100. This is an error. Investigate and correct it. If the real score is unknown, delete this record.

**Step 2 — Handle missing data:** Fatima's score is blank. Calculate the average of the other valid scores: (85 + 78 + 70) ÷ 3 = 77.7. Use 78 as an estimate for Fatima's missing score, or contact the teacher for the real value.

**Step 3 — Investigate outliers:** Bilal's score of 3 is extremely low. Is this real or an error? Investigate. If confirmed real, keep it but note it. If it is an entry error (maybe the real score is 73), correct it.

**Step 4 — Verify consistency:** Are all names spelled consistently? Is the date format the same throughout?

**Clean dataset after processing:**

| Student | Score |
|---------|-------|
| Ali | 85 |
| Ahmed | 78 |
| Fatima | 78 *(estimated)* |
| Bilal | 73 *(corrected)* |

---

#### ✋ Interactive Stop-Point: Pause & Think

Here is a messy dataset of student ages:

| Student | Age |
|---------|-----|
| Zara | 14 |
| Hamza | 150 |
| Noor | 13 |
| Usman | (blank) |
| Hina | 14 |

1. Which value is clearly an **error**? What would you do with it?
2. Which value is **missing**? How would you handle it?
3. After cleaning, what does your corrected dataset look like?

---

### 6.6.4 Data Analysis Techniques

---

#### 📖 Two Types of Data Analysis

After pre-processing, you can analyze the data. There are two main types:

---

**Quantitative Analysis**

> **Definition:** Quantitative analysis deals with **numbers and measurable data**. It uses mathematics and statistics to find patterns, relationships, and trends.

**Common techniques:**
- **Calculating averages:** What is the average test score of the class?
- **Finding maximum/minimum:** Who scored highest? Who scored lowest?
- **Counting:** How many students passed? How many failed?
- **Percentages:** What percentage of students scored above 80?
- **Trends:** Did scores improve from the first test to the second?

**Example:** You have test scores for 30 students. Quantitative analysis tells you:
- Average score: 76
- Highest score: 95
- Lowest score: 42
- Students who scored above 80: 8 (27%)

---

**Qualitative Analysis**

> **Definition:** Qualitative analysis deals with **non-numeric data** — text, images, audio, and experiences. It helps us understand meanings, opinions, and patterns in words.

**Common techniques:**
- **Theme identification:** Reading 50 student feedback forms and identifying the most common themes (e.g., "The classroom is too hot." appears in 30 forms → **temperature** is a theme).
- **Pattern finding:** Noticing that most negative feedback uses words like "boring" or "confusing."
- **Content analysis:** Categorizing responses into groups.

**Example:** You ask 30 students: "How do you feel about online classes?" The answers are qualitative (sentences and opinions). Qualitative analysis reveals that 20 students feel "disconnected" and 15 mention "internet problems" as the biggest challenge.

---

#### ✋ Interactive Stop-Point: Grab a Partner

Your school conducted a survey with two questions:

**Question 1 (Quantitative):** "How many hours do you study per day?" (Average answer: 2.3 hours)

**Question 2 (Qualitative):** "What do you find most challenging about studying?" (Common answers: "Distractions from phone", "Difficult vocabulary in textbooks", "No quiet place at home")

1. What can you conclude from the **quantitative** data?
2. What can you conclude from the **qualitative** data?
3. Which type of analysis gives you more **actionable insight** about how to help students? Discuss.

---

#### 📌 Quick Recap

> **Data pre-processing cleans dirty data — fixing errors, filling missing values, and removing outliers. Quantitative analysis works with numbers; qualitative analysis works with words and experiences. Both are essential for drawing accurate conclusions.**

---

## 6.7 Cloud Storage and Data Backups

### Working Together, Anywhere in the World

---

#### 🔖 The Hook

In 2011, a student named Waqar spent three weeks writing his final year project on his laptop. The night before submission, his laptop crashed. The hard drive was dead. Three weeks of work — gone.

His classmate Sana had the same assignment. She had been saving her work to **Google Drive** every 30 minutes. When her laptop crashed the same night, she simply opened Google Drive on the school computer and continued from exactly where she left off.

**The difference between Waqar and Sana was cloud storage.**

---

### 6.7.1 Cloud Storage for Data Management

---

#### 📖 The Explanation

> **Definition:** Cloud storage means saving files on the **internet** (on remote servers) instead of only on your local device. You can access these files from any device, anywhere, at any time.

Think of cloud storage like an **infinite online bookshelf**. Instead of keeping all your books (files) only in your bedroom (local device), you keep copies on a giant shelf in the sky that you can access from your bedroom, your school, your friend's house — anywhere with an internet connection.

**Popular cloud storage services:**

| Service | Provider | Free Storage |
|---------|---------|-------------|
| **Google Drive** | Google | 15 GB free |
| **OneDrive** | Microsoft | 5 GB free |
| **Dropbox** | Dropbox Inc. | 2 GB free |
| **iCloud** | Apple | 5 GB free |

**Benefits of cloud storage:**

| Benefit | Explanation |
|---------|-------------|
| **Access from anywhere** | Open your files on any device with internet. |
| **Never lose data** | Files survive even if your device breaks. |
| **Share easily** | Send a link to anyone to share a file instantly. |
| **Collaborate** | Multiple people can work on the same file simultaneously. |
| **Automatic saving** | Many cloud services save your work continuously. |

---

### 6.7.2 Remote Access

---

#### 📖 The Explanation

> **Definition:** Remote access is the ability to connect to and use a computer or network from a **distant location** — without being physically present.

**Example:** A student in Lahore can access files stored on a school server in Islamabad using remote access tools. A teacher can review and edit student submissions from home.

**Common remote access tools:**
- **Google Drive** — access and edit files stored online.
- **Microsoft Teams** — access shared files and communicate remotely.
- **Remote Desktop** — control another computer entirely from a different location.

**Why remote access matters:**
- Students can work from home during holidays or illness.
- Teams can collaborate across cities or countries.
- During COVID-19, remote access tools like Zoom and Google Classroom kept education running worldwide.

---

### 6.7.3 Data Backups

---

#### 📖 The Explanation

> **Definition:** A data backup is a **copy of important data stored separately** from the original, used to recover data if the original is lost, deleted, or damaged.

Think of a backup like a photocopy of an important document. If you lose the original, the photocopy saves you.

**When do you need a backup?**
- Your device's hard drive fails.
- You accidentally delete a file.
- A virus corrupts your data.
- Your device is stolen.
- A natural disaster destroys your equipment.

**Three types of backup:**

| Type | What It Does | Example |
|------|-------------|---------|
| **Full Backup** | Copies all data every time. | Copying everything to an external hard drive weekly. |
| **Incremental Backup** | Copies only data that changed since the last backup. | Google Drive saving only the changes you made today. |
| **Automatic Backup** | The system backs up data regularly without you doing anything. | iCloud automatically backing up your iPhone every night. |

**Best practice: The 3-2-1 Rule:**
- Keep **3 copies** of your data.
- Store on **2 different types of media** (e.g., laptop + USB drive).
- Keep **1 copy offsite** (e.g., in the cloud or at a different location).

---

#### 📝 Step-by-Step: Backing Up a School Project

**Step 1:** Complete your work and save it on your laptop.

**Step 2:** Open Google Drive (drive.google.com) and sign in.

**Step 3:** Click **New → File Upload** and upload your project file.

**Step 4:** Confirm the file appears in Google Drive.

**Step 5:** Also copy the file to a USB drive for a second backup.

Now you have three copies: on your laptop, on Google Drive, and on your USB. Even if two fail, the third saves you.

---

### 6.7.4 Benefits of Collaborative Tools

---

#### 📖 The Explanation

Collaborative tools allow multiple people to work on the same document, spreadsheet, or presentation at the same time — from different locations.

**Example:** Three students — one in Lahore, one in Karachi, and one in Peshawar — are working together on a science project. Using Google Docs, all three can type, edit, and comment on the same document simultaneously. Each sees the others' changes in real time.

**Key benefits:**

| Benefit | Explanation |
|---------|------------|
| **Enhanced Productivity** | Multiple people working simultaneously means the project gets done faster. |
| **Version Control** | Google Docs saves every change automatically. You can go back to any previous version at any time. |
| **Real-Time Collaboration** | See what your teammates are typing as they type it. |
| **Global Reach** | A student in Pakistan can collaborate with peers in the USA and Australia on the same project, at the same time. |
| **No Email Required** | Instead of emailing files back and forth (and losing track of versions), everyone works in one shared file. |

---

#### ✋ Interactive Stop-Point: Pause & Think

Your family's computer crashes and all your school project files are lost.

1. What could you have done to prevent this?
2. List three specific places where you could have stored backups.
3. Which of these three is the **safest** option? Why?

Now create a personal backup plan for your school work. What will you back up? How often? Where?

---

#### 📌 Quick Recap

> **Cloud storage saves files on the internet for access from anywhere. Data backups are separate copies of your data stored to protect against loss. Collaborative tools allow multiple people to work on the same files simultaneously — increasing speed, safety, and teamwork.**

---

## 6.8 Introduction to Data Science

### The Science of Finding Answers in Data

---

#### 🔖 The Hook

Netflix knows what show you want to watch before you even search for it. Spotify creates a playlist that feels like it was made specifically for you. Amazon suggests products you were already thinking about buying.

How do these companies do it?

They use **data science**.

They collect millions of data points about what you watch, what you skip, what you pause, what you search — and they use algorithms and analysis to predict what you want next.

Data science is not magic. It is a systematic process of turning raw data into useful knowledge — and it is one of the fastest-growing fields in the world.

---

### 6.8.1 Understanding Data Science

---

#### 📖 The Explanation

> **Definition:** Data science is an interdisciplinary field that uses computer science, mathematics, and domain knowledge to **collect, process, analyze, and interpret large amounts of data** to find patterns and generate useful insights.

Think of a data scientist as a **detective**. Instead of solving crimes, they solve problems — using data as their evidence.

**Example problem:** Why do some students perform better in exams than others?

A data scientist would:
1. **Collect data** — study hours, attendance, sleep patterns, family income, teacher quality.
2. **Clean the data** — remove errors and missing values.
3. **Analyze the data** — look for patterns. (Students who study 3+ hours daily score 15% higher on average.)
4. **Interpret the findings** — students who study in groups score higher than those who study alone.
5. **Make recommendations** — introduce group study sessions as part of the school program.

**Where is data science used?**

| Domain | How Data Science Helps |
|--------|----------------------|
| **Healthcare** | Predicting which patients are at risk of disease. |
| **Sports** | Analyzing player performance to build better teams. |
| **Business** | Predicting which products will sell best next month. |
| **Education** | Identifying students who need extra support before they fail. |
| **Finance** | Detecting fraudulent bank transactions in real time. |
| **Weather** | Predicting rain and storms days in advance. |

---

### 6.8.2 The Interdisciplinary Nature of Data Science

---

#### 📖 The Explanation

Data science is unique because it is built on the intersection of **three different fields**:

```
        Computer Science
              /\
             /  \
            /    \
           /      \
          /  DATA  \
         /  SCIENCE \
        /____________\
   Mathematics    Business
   & Statistics   Knowledge
```

| Field | What It Contributes |
|-------|-------------------|
| **Computer Science** | Writing programs to collect, store, and process data. Using tools like Python and SQL. |
| **Mathematics & Statistics** | Calculating averages, finding patterns, building models, measuring uncertainty. |
| **Business / Domain Knowledge** | Understanding what the data means in context. Knowing which questions to ask and which answers are actionable. |

**Example:** A hospital wants to predict which patients are likely to develop diabetes in the next five years.

- **Computer Science:** Build a program that processes 50,000 patient records.
- **Mathematics:** Build a model that identifies patterns in blood sugar levels, weight, and family history.
- **Medical Knowledge:** Understand which patterns are medically significant and what recommendations to make.

Without all three, the solution is incomplete.

---

#### ✋ Interactive Stop-Point: Pause & Think

Think of a problem in your school that could be solved using data science.

For example: "Why do students perform worse in the second term compared to the first?"

1. What **data** would you need to collect?
2. What **analysis** would you perform?
3. What **insights** might you find?
4. What **action** would you recommend based on those insights?

Discuss with your partner. Present your idea to the class.

---

### 6.8.3 Tools in Data Science

---

#### 📖 The Tools

Professional data scientists use a range of tools. Here are the most important ones — and what they do:

---

**Tool 1: Microsoft Excel**

> **What it is:** A spreadsheet program that organizes and analyzes data using rows, columns, formulas, and charts.

**What you can do with it:**
- Enter and organize data in tables.
- Calculate averages, totals, and percentages using formulas.
- Create bar charts, pie charts, and line graphs with one click.
- Sort and filter data to find what you need.

**Example:** You have 30 students' test scores. In Excel, you can calculate the class average in two seconds using the formula `=AVERAGE(B2:B31)`. You can then create a bar chart showing each student's score.

**Best for:** Students and beginners. Excel is the most widely used data tool in the world.

---

**Tool 2: Python**

> **What it is:** A programming language that is extremely popular in data science because of its simplicity and powerful libraries.

**Key libraries in Python for data science:**

| Library | What It Does |
|---------|-------------|
| **Pandas** | Organizes and manipulates data in tables (called DataFrames). |
| **Matplotlib** | Creates charts and graphs from data. |
| **NumPy** | Performs mathematical calculations on large datasets. |
| **Scikit-learn** | Builds machine learning models to make predictions. |

**Example:** You have a CSV file with survey results from 5,000 students. Python (with Pandas) can load all 5,000 records in one line of code, calculate statistics in seconds, and create a visualization in a few more lines — something that would take hours to do manually in Excel.

**Best for:** Intermediate and advanced users who work with large datasets or want to build predictive models.

---

**Tool 3: R**

> **What it is:** A programming language specifically designed for **statistical analysis** and data visualization.

**What R is best at:**
- Advanced statistical tests (t-tests, regression analysis, ANOVA).
- Creating complex, publication-quality graphs and plots.
- Handling large statistical datasets from scientific research.

**Example:** A medical researcher analyzes data from a clinical trial with 10,000 patients. R is used to run statistical tests that determine whether a new drug is significantly more effective than the existing one.

**Best for:** Scientific research, statistics, and academic data analysis.

---

**Tool 4: SQL (Structured Query Language)**

> **What it is:** A language used to **manage and query databases** — to search for, retrieve, and organize data stored in structured databases.

**Think of SQL like this:** Imagine a huge library with millions of books (records). SQL is how you ask the librarian for specific books: *"Show me all books by the author 'Ali Ahmed' published after 2020."*

**Common SQL commands:**

| Command | What It Does | Example |
|---------|-------------|---------|
| `SELECT` | Retrieve data from a database | `SELECT Name, Score FROM Students` |
| `WHERE` | Filter results by condition | `WHERE Score > 80` |
| `ORDER BY` | Sort results | `ORDER BY Score DESC` |
| `INSERT` | Add new records | `INSERT INTO Students VALUES (...)` |

**Example:** A school database has 1,000 student records. Using SQL, the admin can instantly find all students in Class 9 who have not paid their fees: `SELECT Name FROM Students WHERE Class='9th' AND FeeStatus='Unpaid'`

**Best for:** Working with large structured databases — essential for any data-related career.

---

#### 📝 Choosing the Right Tool

| Situation | Best Tool |
|-----------|----------|
| Creating a chart for a class project | Excel or Google Sheets |
| Analyzing 100 survey responses | Excel or Google Sheets |
| Analyzing 100,000 survey responses | Python (Pandas) |
| Running advanced statistical tests | R |
| Searching a large database of records | SQL |
| Building a system to recommend songs | Python (Scikit-learn) |

---

#### ✋ Interactive Stop-Point: Pause & Think

Match each scenario to the best data science tool:

1. A school admin wants to find all students who scored below 50 in the last exam from a database of 800 students.
2. A student wants to create a pie chart of their survey results (50 responses) to present to class.
3. A data scientist wants to analyze 1 million tweets to find what topics people discuss most.
4. A scientist wants to run a complex statistical test on medical trial data with 5,000 patients.

Which tool — Excel, Python, R, or SQL — fits each scenario best? Justify your choice.

---

#### 📌 Quick Recap

> **Data science combines computer science, mathematics, and domain knowledge to solve real problems using data. Key tools include Excel for beginners, Python for large-scale analysis, R for statistics, and SQL for database queries.**

---

## Chapter Summary

| Topic | Key Takeaway |
|-------|-------------|
| **Data** | Raw facts collected about the world. Must be processed to become useful information. |
| **Qualitative Data** | Describes qualities in words — non-numeric, categorical. Answers "what kind?" |
| **Quantitative Data** | Measured in numbers — countable and calculable. Answers "how many?" |
| **Data Organisation** | Tables, charts, and graphs make data easier to read and analyze. |
| **Data Collection Methods** | Surveys, questionnaires, interviews, observations, online sources. |
| **Structured Data** | Organised in rows and columns — easy to search and calculate. |
| **Unstructured Data** | Free-form — emails, images, videos. Harder to analyze, but most common. |
| **Data Visualization** | Turning data into charts and graphs. Bar charts compare; pie charts show proportions; line graphs show trends. |
| **Visualization Tools** | Excel, Google Sheets (beginner); Tableau, Power BI (advanced). |
| **Data Pre-Processing** | Cleaning raw data — fixing errors, filling missing values, handling outliers. |
| **Data Validation** | Checking data is complete and accurate before analysis. |
| **Data Cleaning** | Removing or correcting errors, duplicates, and outliers. |
| **Quantitative Analysis** | Analyzing numbers — averages, totals, percentages, trends. |
| **Qualitative Analysis** | Analyzing text and experiences — finding themes, patterns, and meanings. |
| **Cloud Storage** | Saving files online for access from any device, anywhere. |
| **Remote Access** | Connecting to files and networks from a distant location. |
| **Data Backups** | Separate copies of data stored to protect against loss. |
| **Collaborative Tools** | Allow multiple people to work on the same files simultaneously (Google Docs, OneDrive). |
| **Data Science** | Using computer science, math, and domain knowledge to find insights in data. |
| **Interdisciplinary** | Data science combines computer science, mathematics, and business/domain knowledge. |
| **Excel** | Best for beginners — charts, formulas, basic analysis. |
| **Python** | Best for large datasets and building models — Pandas, Matplotlib. |
| **R** | Best for advanced statistics and scientific analysis. |
| **SQL** | Best for querying and managing structured databases. |

---

## Key Vocabulary

| Term | Definition |
|------|-----------|
| **Data** | Raw facts collected from the world that can be processed into useful information. |
| **Qualitative Data** | Non-numeric data that describes qualities, categories, or characteristics. |
| **Quantitative Data** | Numeric data that measures quantities, amounts, or counts. |
| **Structured Data** | Data organised in a fixed format of rows and columns; easy to search and analyze. |
| **Unstructured Data** | Free-form data with no fixed format — emails, images, videos, social media posts. |
| **Data Visualization** | The process of representing data as charts, graphs, and maps for easier understanding. |
| **Data Pre-Processing** | Cleaning and organising raw data before analysis. |
| **Data Validation** | Checking that data is complete and accurate. |
| **Data Cleaning** | Removing or correcting errors, missing values, and outliers in a dataset. |
| **Outlier** | An unusual or extreme data value that does not fit the pattern of the rest of the data. |
| **Bias** | A distortion in data that makes it unrepresentative of the full population. |
| **Quantitative Analysis** | Analysis that uses numbers and statistics to find patterns and trends. |
| **Qualitative Analysis** | Analysis that examines text, images, and experiences to find meanings and themes. |
| **Cloud Storage** | Storing files on remote internet servers, accessible from any device. |
| **Remote Access** | The ability to connect to and use a computer or network from a distant location. |
| **Data Backup** | A separate copy of data stored to recover from accidental loss or damage. |
| **Collaborative Tools** | Software that allows multiple users to work on the same files simultaneously. |
| **Data Science** | An interdisciplinary field combining computer science, mathematics, and domain knowledge to extract insights from data. |
| **SQL** | Structured Query Language — used to manage and query structured databases. |
| **Python** | A programming language widely used in data science for analysis and modelling. |
| **R** | A programming language designed for statistical analysis and data visualization. |
| **Survey** | A method of collecting data by asking a group of people standardized questions. |
| **Questionnaire** | A written set of questions used to collect structured data from respondents. |
| **Bar Chart** | A chart that uses vertical or horizontal bars to compare quantities across categories. |
| **Pie Chart** | A circular chart divided into slices to show proportions of a whole. |
| **Line Graph** | A graph that connects data points with a line to show change over time. |

---

## Review Questions

### Multiple Choice Questions

1. What is data?
   - a) Processed information ready to use
   - b) **Raw facts gathered about things around us**
   - c) A collection of numbers only
   - d) A list of observed events

2. Which of the following is an example of qualitative data?
   - a) Temperature readings in degrees Celsius
   - b) Number of students in a class
   - c) **Favourite ice cream flavours**
   - d) Test scores out of 100

3. Which of the following is an example of quantitative data?
   - a) Colour of a car
   - b) Name of a city
   - c) Blood group
   - d) **Height of a student: 165 cm**

4. How can you best organise data for analysis?
   - a) Write it in long paragraphs
   - b) **Create tables, charts, and graphs**
   - c) Store it in random files
   - d) Keep it in a messy notebook

5. What is the primary purpose of data visualization?
   - a) To generate random numbers
   - b) To convert text into data
   - c) **To make data easier to understand by turning it into pictures**
   - d) To hide complex data

6. Which tool is specifically designed for creating detailed and interactive visualizations?
   - a) Microsoft Excel
   - b) Google Sheets
   - c) **Tableau**
   - d) PowerPoint

7. What is the first step in working with data before analysis?
   - a) Data Analysis
   - b) Data Cleaning
   - c) **Data Pre-Processing**
   - d) Data Visualization

8. Which type of data is stored in rows and columns and is easy to search?
   - a) Unstructured data
   - b) Qualitative data
   - c) Raw data
   - d) **Structured data**

9. A backup is best described as:
   - a) The original copy of a file
   - b) A program that speeds up data analysis
   - c) **A separate copy of data stored to protect against loss**
   - d) A cloud storage service

10. Which programming language is most commonly used in data science for large-scale analysis?
    - a) SQL
    - b) R
    - c) Excel
    - d) **Python**

---

### Short Questions

1. Write two differences between qualitative and quantitative data.
2. Which data collection method would you use to collect opinions from a large group of people about a new school policy? Justify your choice.
3. What type of data is "the number of students in your class"?
4. Why is it important to organise data into tables or charts before analyzing it?
5. Explain why data visualization is important. Give one real-world example.
6. For what purpose do we use a line graph? Give an example.
7. How does Microsoft Power BI help in data visualization?
8. What is Python? How is it used in data science?
9. What is SQL? Give one example of when it would be used.
10. Differentiate between structured and unstructured data. Give one example of each.
11. What is data pre-processing? Why is it necessary?
12. Define an outlier. Give one example from a school context.
13. What is data validation? Give two examples of validation checks.
14. What is cloud storage? Name two cloud storage services.
15. What is a data backup? Why is it important to maintain backups?
16. List two benefits of using collaborative tools like Google Docs.
17. Define data science in your own words.
18. What are the three fields that data science combines?
19. Differentiate between quantitative analysis and qualitative analysis.
20. What is the difference between a survey and a questionnaire?

---

### Long Questions

1. Define data. Explain the difference between qualitative and quantitative data with at least three examples of each. Why is it important to identify the correct data type before analysis?

2. Describe five methods of data collection. For each method, explain how it works, give a real-world example, and state when it is most appropriate to use.

3. Explain the importance of organising data. Describe three ways to organise data (tables, charts, graphs) and explain when each is most useful. Include descriptions of at least two types of charts.

4. What is data visualization? Describe four types of charts or graphs (bar chart, pie chart, line graph, scatter plot). For each, explain what it is best used for and how to construct it. Name two tools used for data visualization and explain their features.

5. What is data pre-processing? Explain the following in detail with examples: (a) Evaluating data quality (b) Identifying errors, outliers, and biases (c) Data validation (d) Data cleaning. Why is the saying "garbage in, garbage out" relevant to data pre-processing?

6. Differentiate between structured and unstructured data. Give three examples of each. What are the challenges of working with unstructured data? Where is each type commonly used?

7. Explain cloud storage and data backups. Why are they important? Describe the 3-2-1 backup rule. List four benefits of cloud storage and explain three benefits of using collaborative tools.

8. What is data science? Explain its interdisciplinary nature — which three fields does it combine and what does each contribute? Using a real-world example, walk through all five steps of the data science process: collect → clean → analyze → interpret → recommend.

9. Describe four data science tools: Microsoft Excel, Python, R, and SQL. For each tool, explain what it is, what it is best used for, and give a practical example of how it is used. For which type of task would you choose each tool?

10. Write a short essay on the role of data science in modern society. In your essay, discuss how data science is used in at least three of the following sectors: healthcare, education, finance, sports, weather forecasting, and retail. For each sector, give a specific example of how data science is making a difference.

---

*End of Unit 6: Data Science and Data Gathering*

---

> **You are now a data thinker.** Every survey result, every cricket scorecard, every weather forecast, every Netflix recommendation — all of it is the result of collecting, cleaning, organizing, and analyzing data. You now know how that process works from start to finish. The world is full of questions. Data is how you find the answers. Go find them.
