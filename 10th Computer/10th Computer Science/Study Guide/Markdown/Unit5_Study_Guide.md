# Unit 5: Data Science

## Student Learning Outcomes

By the end of this chapter, you will be able to:

- Explain the concept and importance of data science in everyday life.
- Describe each step in the Data Science Life Cycle (DSLC).
- Identify and define real-world problems that can be solved using data.
- Collect data using surveys, online forms, and observational techniques.
- Perform data cleaning and validation to improve accuracy.
- Use simple SQL queries (SELECT, INSERT) to retrieve and store data from databases.
- Analyze data using basic algorithms (sorting, classification, clustering).
- Create bar charts and dashboards to visually represent data insights.
- Communicate results clearly using charts and written summaries.

---

## Introduction

Here's a strange fact: right now, while you're reading this sentence, data is being generated somewhere about you. Your phone knows how long you scrolled today. Your fitness tracker knows how many steps you took. Your school's attendance register knows exactly which days you were late.

Data by itself is just numbers and words sitting quietly, doing nothing. **Data Science** is what happens when someone picks up that pile of numbers and asks it smart questions — until it starts revealing patterns nobody could see at first glance.

In this digital era, data is everywhere: surveys, mobile apps, social media, online shopping, health services. Data Science helps us turn this raw data into useful information. Whether it's predicting weather, understanding student interests, or improving healthcare, Data Science is quietly transforming how we live, learn, and work. Organizations across the world use data to improve decision-making, save costs, and build better services.

This chapter introduces the **Data Science Life Cycle (DSLC)** — a series of steps that takes you from "I have a messy pile of numbers" all the way to "Here's a clear chart that explains exactly what's going on." Each step builds critical thinking and problem-solving skills you'll use far beyond this classroom.

You will also learn how to collect, clean, analyze, interpret, and visualize data using simple, familiar tools like surveys, spreadsheets, and charts. Real-world examples and hands-on activities will help you apply Data Science in your classroom and daily life — starting today.

---

## 5.1 Introduction to Data Science

### The Hook (Story Mode)

In 1854, a deadly cholera outbreak swept through a neighborhood in London, killing people by the dozens. At the time, doctors believed diseases spread through "bad air." A physician named **Dr. John Snow** wasn't convinced. Instead of guessing, he did something radical for his time: he collected data. He walked door to door, marking a small dot on a map for every single death in the neighborhood.

When he stepped back and looked at his map, a pattern jumped out that no one had noticed before — the dots clustered tightly around one specific water pump on Broad Street. Snow convinced local officials to remove the pump's handle. The outbreak collapsed almost immediately.

Dr. Snow didn't have a computer, a spreadsheet, or a single line of code. He had raw data, turned into a visual pattern, and it saved thousands of lives. That map is now considered the birth of modern data visualization — and it's proof that data science isn't really about fancy technology. It's about asking the right question of the right information.

### The Explanation

We are living in a world full of data. Whether we're using a mobile phone, searching on Google, shopping online, or walking around with a fitness tracker, data is quietly being collected around us all the time. So the real question is: **how is this data actually useful?**

**Data Science** is the field where we use data to find patterns, answer questions, and help people or businesses make better decisions. It involves collecting, organizing, analyzing, and visualizing data.

**Importance of Data in Decision Making**

Data plays a huge role in helping people and organizations make better decisions. Without data, decisions are often based on guesses or personal opinions — and guesses can be wrong. For example, if a school's administration wants to start a new sports club, they could just guess what students like. Or, they could first collect data on which sports students actually enjoy most. That second option leads to a smarter, fairer choice.

Here's a modern example of the same idea, at a much bigger scale: before Netflix filmed its very first original show, *House of Cards*, the company already had years of data about its users — what they paused, what they rewound, which genres and actors they watched again and again. By studying that data carefully, Netflix was confident the show would be a hit *before a single scene was filmed*. That's the power of using data instead of guessing.

**Real-Life Applications of Data Science**

Data Science is used in many aspects of our daily life, often without us even noticing:

- **Social media:** Apps like Facebook, YouTube, and Instagram use data to show us posts or videos we're likely to enjoy.
- **Online shopping:** E-commerce websites suggest products based on data from our previous purchases.
- **Healthcare:** Hospitals use data science to predict diseases and manage patient care more effectively.
- **Transport:** Apps like Google Maps use traffic data to suggest the fastest available route.
- **Education:** Schools use data from student attendance and test results to improve learning strategies and track progress.

Data Science supports making our lives smarter, easier, and more personalized — from the videos you watch on YouTube, to the health tips you receive, to the route your rickshaw driver takes to avoid traffic.

### The Practical Walkthrough

Let's practice spotting data science in action, step by step, using something you do almost every day: opening YouTube.

1. **Notice the Raw Data Being Collected** — Every video you watch, pause, skip, or rewatch is quietly recorded as a small piece of data.
2. **Imagine It Piling Up** — Multiply that by millions of users, watching billions of videos, every single day. That mountain of numbers is the "raw material" data scientists work with.
3. **Ask the Smart Question** — A data scientist at YouTube might ask: "Which videos do people similar to this user tend to watch next?"
4. **Find the Pattern** — By comparing your habits to millions of other viewers with similar habits, the system finds a pattern — say, viewers who watch cricket highlights often also watch cricket analysis videos.
5. **Turn the Pattern into a Decision** — YouTube uses that pattern to recommend your next video, right there on your homepage.

**What just happened?** You just traced the invisible data science pipeline running quietly behind one of the most familiar apps on your phone — from raw data, to pattern, to decision.

### Interactive Stop-Point

**Pause & Think — 5.1:** Imagine you want to find out the most popular video game in your school. If you only ask the members of the "Action Gamers Club," why might your data lead to a terrible decision? What might you be missing?

### Quick Recap

Data Science turns raw, everyday data into patterns we can actually use — and smart decisions built on real data almost always beat decisions built on guesses.

---

## 5.2 Overview of the Data Science Life Cycle

### The Hook (Story Mode)

Picture this: it's Friday afternoon, and the school library is completely empty — again. The librarian is frustrated but doesn't know why. She could guess ("maybe students just don't like reading"), or she could follow a clear process to actually find out.

That process — Problem, Collection, Analysis, Interpretation, Visualization — is exactly what data scientists everywhere follow, whether they're studying an empty library or a billion-dollar business. It's called the **Data Science Life Cycle**, and once you learn its steps, you can apply them to almost any mystery in your life.

### The Explanation

Data Science is not completed in a single step. It follows a series of steps that help us solve a problem properly. This is what we call the **Data Science Life Cycle (DSLC)**.

The DSLC usually comprises the following six steps:

- **Step 1:** Understanding the Problem
- **Step 2:** Collecting Data
- **Step 3:** Cleaning and Validating Data
- **Step 4:** Analyzing Data
- **Step 5:** Interpreting Data
- **Step 6:** Visualizing and Communicating Results

**Note:** The standard DSLC has these 6 main steps. However, in real-world projects — especially large ones, or projects involving teams — an additional step is often added: **Storing and Organizing Data**, usually managed through databases and SQL. We'll cover that later in this chapter, in Section 5.4.

#### Understanding the Problem

Before we even think about collecting data, we must clearly understand the problem. This is the most important step in the entire DSLC. If we don't understand the problem properly, we may end up collecting the wrong data — leading to useless or misleading results.

In this initial step, we ask questions like *what, why,* and *who*:

- What are we trying to find out?
- Why is this problem important?
- Who will use the results?

**Identifying and Defining a Problem**

First, we identify a problem we want to solve using data. It can be related to school, home, city, or any area of life where decisions are made based on information. Once identified, the problem must be defined clearly and simply.

**Example:** Instead of saying vaguely, "students are not happy," we can define the problem better as: **"Which school activities do students enjoy the most?"**

When defining a problem, consider:

1. Use clear and simple words.
2. Focus on one specific question.
3. Avoid unclear or overly general terms.

> **TIDBIT:** A good problem is one that can be answered by collecting and analyzing data.

**Setting Clear Objectives**

Once the problem is identified and defined, we must decide what we want to achieve. These are our **objectives** — they guide the rest of the data science process by stating: (i) what kind of data we need, (ii) what questions we will ask, and (iii) what results we are looking for.

**Example:** For the problem "Which school activities do students enjoy the most?", our objectives could be:

- Find out how many students participate in each activity.
- Find out which activity is rated as most enjoyable by students.
- Recommend which activities should be improved or replaced.

> **TIDBIT:** Write your objectives like a checklist. This helps keep your project focused.

**Table 5.1: Example Problems and Objectives**

| Domain | Example Problem | Objectives |
|---|---|---|
| **School** | Many students arrive late at school. | Find out how many students arrive late each month. Identify reasons for being late (e.g., transport, distance, emergency, weather). Suggest solutions to reduce late arrivals. |
| **Health** | Many students are not drinking enough water during school hours. | Collect data on how much water students drink daily. Find out reasons for low water intake. Recommend steps to promote healthy habits. |
| **Business** | A school canteen wants to know which snacks students like most. | Survey students on their favorite snacks. Compare popularity and sales data. Help the canteen manager make smarter ordering decisions. |

> **REMEMBER:**
> 1. The first step in any data science project is to understand the problem.
> 2. We must define the problem clearly and set specific goals.
> 3. Clear problems are solvable using data.
> 4. Clear objectives help in collecting the right data and reaching useful results.

#### Collecting Data

Once we understand the problem and set clear goals, the next step in the DSLC is to collect the required data. Data is like raw material — we must gather the right kind before we can clean, store, or analyze it.

In Step 1, we asked questions like "Which school activities do students enjoy the most?" Step 2 is about actually collecting information that can help answer these questions. We will explore: (i) data collection methods, (ii) where to collect data from (sources), and (iii) how to make sure the data is useful and fair (data quality).

**(i) Methods of Data Collection**

There are many ways to collect data, depending on the problem and tools available:

- **Surveys (Online/paper-based):** The easiest and most common method. We ask people questions and record their answers. *Example:* To find out which sports students enjoy, we might ask: (i) Which sport do you like the most? (ii) How often do you play it? (iii) What time of day do you prefer to play?

  > **DO YOU KNOW?** Surveys can be done using Google Forms (online) or printed paper forms (manual).

- **APIs and Online Sources:** An **Application Programming Interface (API)** allows software to collect data from websites or apps automatically. *Example:* A school may use an attendance API to automatically pull daily attendance data into a report. (More commonly used by developers.)

- **IoT and Sensor Data:** **Internet of Things (IoT)** devices like smart watches, water dispensers, or temperature sensors can automatically collect data. *Example:* To study water-drinking habits, a school could place smart water meters near fountains.

  > **TIDBIT:** IoT devices are especially useful in health, safety, and environmental monitoring.

- **Web Scraping:** The process of programmatically collecting public data from websites. *Example:* A business student might scrape snack prices from online stores to compare them with school canteen prices.

  > **TIDBIT:** Web scraping should only be done with a teacher's guidance, and only on websites that allow it.

**(ii) Choosing the Right Data Source**

Not all data is useful. We must choose reliable, accurate, and relevant sources. Before using a source, ask: (i) Is this data from a trusted place? (ii) Is it recent or outdated? (iii) Does it match the problem I want to solve?

**Example:** If we want to know students' favorite snacks in 2025, we should avoid using a survey conducted back in 2020 — it's simply too outdated.

> **TIDBIT:** Always collect fresh, problem-related data.

**(iii) Assessing Data Quality and Bias**

**Data quality** means the data is: (i) **Complete** (no missing values), (ii) **Correct** (no mistakes), and (iii) **Relevant** (matches our problem).

**Bias** means the data only shows part of the truth and misses the full picture. For example, if we only survey boys about their favorite sports, we miss the opinions of girls entirely — and the results will be unfair, or *biased*, toward boys.

To avoid bias:

- Ask a diverse group of people.
- Keep questions neutral, not leading.
- Review answers for strange or suspicious patterns.

> **REMEMBER:**
> 1. After defining a problem, we need to collect data that can help solve it.
> 2. There are different methods of data collection: surveys, APIs, sensors, and web scraping.
> 3. We should always check for data quality and fairness (bias) before moving to the next step.
> 4. Data that is incomplete or biased can lead to wrong decisions.

#### Cleaning and Validating Data

After collecting data, the next important step is to clean and validate it. Raw data is often messy — it may contain errors, missing values, or wrong entries. If we use messy data without checking it, our analysis will give wrong results.

Here's something every data professional wants you to know early: **cleaning messy data isn't a sign that something went wrong.** It's completely normal. In fact, professional data scientists often spend around 80% of their time just cleaning and organizing data before they ever get to the "exciting" analysis part. If your first survey table looks like a mess, congratulations — you're having a completely authentic data science experience.

**Raw Data**

**Raw data** is the original information we collect from people, sensors, websites, or apps. It has not been checked or cleaned yet.

**Table 5.2: Raw Data about Favorite Sport of Students**

```
+----+-------+----------------+-----------+----------------+
| ID | Name  | Favorite Sport | Frequency | Time of Day    |
+----+-------+----------------+-----------+----------------+
| 1  | Ahmad | cricket        | Daily     | Evening        |
| 2  | Ali   |                | Weekly    |                |
| 3  | Sara  | Footbal        |           | Evening        |
| 4  | Sana  | Football       | Daliy     | Afternoon      |
+----+-------+----------------+-----------+----------------+
```

Table 5.2 contains several problems:

- **Spelling errors:** "Footbal" (ID 3), "Daliy" (ID 4)
- **Missing entries:** blank Favorite Sport for ID 2, blank Frequency and Time of Day for ID 2/3
- **Mixed capitalization:** "cricket" (ID 1) vs. "Football" (ID 4)

Data like this needs cleaning before it can be trusted.

**Common Data Errors (Missing, Duplicate, Outliers)**

**Table 5.3: Common Issues in Raw Data**

| Error Type | Example |
|---|---|
| Missing data | Blank cells (e.g., no sport name or study time of day) |
| Duplicate entries | Same student entered twice |
| Inconsistent formats | "Cricket", "cricket", "CRICKET" |
| Spelling mistakes | "Footbal", "Daliy" |
| Outliers (strange values) | Frequency = "1000 times/week" |

**Data Validation Techniques**

**Data validation** means checking if the data: (i) follows correct rules (e.g., only valid sport names), (ii) has the right type of values (e.g., numbers where numbers are expected), and (iii) is not fake or nonsensical.

**Example Validation Rule:** Only allow one of these values for "Favorite Sport": Football, Cricket, Badminton, Hockey.

**Validation in Surveys:**

- Use multiple choice instead of blank text boxes.
- Make important questions required, so no one skips them.
- Use dropdowns or checkboxes to reduce spelling mistakes.

> **TIDBIT:** Tools like Google Sheets and Excel provide built-in validation rules that can help catch bad data before it's even entered.

**Data Cleaning Methods**

Once we find mistakes, we need to fix or remove them. This is called **data cleaning**. Common steps include:

1. **Fix spelling errors:** "Footbal" → "Football"
2. **Standardize formats:** "CRICKET" → "Cricket"
3. **Remove duplicates (redundancy):** Delete repeated entries for the same student.
4. **Handle missing values:** Ask the person again, OR remove the row.
5. **Fix invalid data:** If frequency is written as "Eten hundred," fix it or remove it.

**Why Cleaning Data Matters**

Suppose we skip this step entirely, and analyze data that still contains misspelled sports ("Cricket"), missing study times, and duplicates. Our result might mistakenly report: **"Football: 3 votes, cricket: 1 vote, Cricket: 2 votes."**

This gives a wrong picture — "cricket" and "Cricket" are the exact same sport, just typed differently! In summary: **clean data leads to smart decisions. Dirty data leads to incorrect results.**

### The Practical Walkthrough

Let's clean Table 5.2 from raw, messy data into a trustworthy, clean table, step by step.

1. **Spot the Spelling Errors** — Look for "Footbal" and "Daliy." These need correcting.
2. **Fix the Spelling** — Change "Footbal" to "Football," and "Daliy" to "Daily."
3. **Spot Inconsistent Capitalization** — Notice "cricket" is lowercase in row 1 while "Football" is capitalized elsewhere.
4. **Standardize Capitalization** — Change "cricket" to "Cricket" so every entry follows the same style.
5. **Spot Missing Values** — Notice ID 2 has no sport listed, and rows 2 and 3 are missing a Time of Day.
6. **Handle Missing Values** — Either go back and ask that student again, or clearly mark the cell as "Missing" so it isn't confused with real data later.

**Cleaned Table 5.2:**

```
+----+-------+----------------+-----------+----------------+
| ID | Name  | Favorite Sport | Frequency | Time of Day    |
+----+-------+----------------+-----------+----------------+
| 1  | Ahmad | Cricket        | Daily     | Evening        |
| 2  | Ali   | Missing        | Weekly    | Missing        |
| 3  | Sara  | Football       | Missing   | Evening        |
| 4  | Sana  | Football       | Daily     | Afternoon      |
+----+-------+----------------+-----------+----------------+
```

**What just happened?** You just transformed messy, unreliable raw data into a clean, consistent table — exactly the kind of table a data scientist would trust enough to analyze.

### Interactive Stop-Point

**Grab a Partner — 5.2 (Cleaning):** Sit with a partner and look at this raw entry: `Name: Zara | Sport: BADMINTON | Frequency: Dali | Time: mornin`. Find all the errors together, and rewrite the row exactly as it should appear in a clean table.

#### Analyzing Data

Now that our data is collected and cleaned, we can move to analysis. This is where we look at the data to find patterns, trends, and answers to the questions asked back in Step 1.

**What Does It Mean to Analyze Data?**

Analyzing data means carefully examining it to:

1. **Summarize it** (e.g., how many students chose each option).
2. **Compare different groups** (e.g., boys vs. girls, morning vs. evening).
3. **Find patterns** (e.g., most students prefer football and play in the evening).

We often use simple measures like **counts** (how many?), **averages**, and **frequency** (how often?).

**Using Simple Tools for Analysis**

You can start analyzing data with simple tools such as Google Sheets, Microsoft Excel, or even manual notebook writing.

**Example:** You surveyed 20 students. Table 5.4 shows what you found.

**Table 5.4: Data Derived from Student Survey**

```
+-----------------+-----------+
| Favorite Sport  | Frequency |
+-----------------+-----------+
| Cricket         | 10        |
| Football        | 5         |
| Hockey          | 4         |
| Badminton       | 1         |
+-----------------+-----------+
```

From this data, we can observe that most students prefer cricket.

> **REMEMBER:**
> 1. Data analysis helps us find patterns and make decisions.
> 2. We use counts and comparisons to understand data.
> 3. Even simple tools like tables or spreadsheets can help us analyze data.

#### Interpreting Data

This step is about finding meaning from data — identifying trends and patterns and asking what they actually mean.

After summarizing the data, ask yourself:

- What do the numbers tell us?
- Why are some options more popular?
- Are there any surprises or patterns?

**Example:** If we find that most late-arriving students live far from school, we can recommend providing transport support as a possible solution.

Here's a relatable everyday version of this exact step: think about your phone's "Screen Time" report. The raw number — say, 4 hours on TikTok yesterday — is just **data**. Realizing you should put your phone away earlier tonight so you sleep better is the **interpretation**. The numbers only become useful once you ask, "So what should I actually do about this?"

#### Visualizing and Communicating Results

After analyzing the data, the final step is to share the results in a way others can easily understand. People generally understand pictures faster than raw numbers — which is exactly why we use **data visualizations**.

Remember, in the previous step we found that cricket was the most popular sport. In this step, we create a chart that shows this clearly, making it easy to present our findings to classmates, teachers, or anyone else.

**Importance of Data Visualization**

Data visualization is important because it:

1. Makes data easier to understand.
2. Shows patterns at a glance.
3. Helps share ideas clearly in presentations or reports.

**Example:** Instead of saying "10 students like cricket," we can show it in a bar chart — something like this simple ASCII version:

```
Cricket   | ########## (10)
Football  | ##### (5)
Hockey    | #### (4)
Badminton | # (1)
          +---------------------
            0   2   4   6   8  10
              Number of Students
```

**Common Types of Charts and Graphs**

Always choose a chart that matches your data. Table 5.7 shows commonly used chart types.

**Table 5.7: Common Types of Charts**

| Chart Type | Used For | Example |
|---|---|---|
| **Bar Chart** | Comparing groups | Number of students who like each sport |
| **Pie Chart** | Showing parts of a whole | Percentage of favorite snacks |
| **Line Chart** | Showing changes over time | Number of students arriving late each week |

> **TIDBIT:** Keep your charts simple, clean, and properly labeled.

**Communicating Results**

Once your chart is ready, explain your findings in a short, clear written summary. For example:

*"Most students (10) like cricket, followed by football (6). Very few students like badminton (1)."*

> **TIDBIT:** Use visuals and words together to tell a data story — clear, short, and useful.

> **REMEMBER:**
> 1. Visualizing data means using charts or graphs to show findings.
> 2. It makes data easier to understand and share.
> 3. Use the right chart for your data type.
> 4. Always label and explain your visuals.

### The Practical Walkthrough

Let's walk through the entire Data Science Life Cycle end-to-end, using a concrete mystery: **"Why is the school library always empty on Fridays?"**

1. **Understand the Problem** — Define it clearly: "How many students visit the library each day of the week, and why is Friday attendance so low?"
2. **Set Objectives** — Decide what we need: (i) daily visitor counts for a full month, (ii) reasons students give for skipping the library on Fridays.
3. **Collect Data** — Hand out a short survey to students, asking which days they usually visit the library, and why they skip certain days.
4. **Clean and Validate** — Check the survey responses for missing answers, fix inconsistent day names (e.g., "fri" vs. "Friday"), and remove obviously fake entries.
5. **Analyze the Data** — Count how many students visit on each day. Suppose the count shows: Monday = 40, Tuesday = 35, Wednesday = 38, Thursday = 33, Friday = 6.
6. **Interpret the Data** — Ask why. Perhaps most students said, "We have sports practice every Friday afternoon," revealing the real cause.
7. **Visualize and Communicate** — Draw a bar chart showing visits per day, with Friday's tiny bar standing out sharply, and write a short summary: *"Library visits drop dramatically on Fridays, mainly due to scheduled sports practice."*

**What just happened?** You just completed a full, real Data Science Life Cycle — from a vague frustration ("the library is empty") to a specific, evidence-backed explanation, using exactly the same six steps professionals use for far bigger problems.

### Interactive Stop-Point

**Pause & Think — 5.2 (Interpreting):** A survey shows that most late-arriving students live far from school. Before jumping to "provide transport support" as the solution, what other reasons might explain this same pattern? Can you think of at least one alternative interpretation?

**Grab a Partner — 5.2 (Visualizing):** Imagine a bar chart comparing two classes' test scores, but the Y-axis starts at 50 instead of 0. Discuss with a partner: how would this make a small difference between the classes look dramatically bigger than it really is? How can graphs "lie" to us if we're not careful?

### Quick Recap

The Data Science Life Cycle — Understand, Collect, Clean, Analyze, Interpret, Visualize — takes you from a vague question to a clear, evidence-based answer that others can easily see and trust.

---

## 5.3 Tools for Visualization

### The Hook (Story Mode)

Think about "Spotify Wrapped" — that yearly summary showing your top songs, top artists, and total minutes listened. Millions of people share it every December because a well-designed chart is genuinely satisfying to look at. But behind that flashy design is the exact same idea Dr. John Snow used with his cholera dot map back in 1854: take numbers, and turn them into something the eyes can instantly understand. The only difference is that today, you don't need to draw dots on paper by hand — you can use free, beginner-friendly software instead.

### The Explanation

Once you know which type of chart to use, the next step is to actually create it using tools. In Step 6 of the DSLC, we learned how charts make data easier to understand and present. In this section, you'll learn how to actually build those charts using software.

**Creating Charts in Spreadsheets (Excel/Google Sheets)**

Google Sheets and Microsoft Excel are simple yet powerful tools for creating charts and graphs from tables of data.

We use spreadsheets because they are:

1. **Easy to use** — no complicated setup required.
2. **No installation needed** (for Google Sheets, which runs entirely in your browser).
3. **Good for small to medium-sized projects**, like a class survey.

### The Practical Walkthrough

Let's turn a simple frequency table into an actual bar chart, step by step, using Google Sheets.

**Starting data (from Table 5.6):**

```
+------------+---------------------+
| Sport      | No. of Students     |
+------------+---------------------+
| Cricket    | 7                   |
| Football   | 6                   |
| Hockey     | 5                   |
| Badminton  | 2                   |
+------------+---------------------+
```

1. **Enter Your Data** — Open Google Sheets and type your data into rows and columns, exactly as shown above: column A for Sport, column B for Number of Students.
2. **Select the Data Range** — Click and drag your mouse to highlight both columns, from the "Sport" header down to the last row ("Badminton").
3. **Open the Insert Menu** — Click on **"Insert"** in the top menu bar, then choose **"Chart."**
4. **Pick the Chart Type** — In the chart editor panel that appears, select **"Bar chart"** (or "Column chart," which shows vertical bars) from the chart type dropdown.
5. **Customize the Chart** — Add a clear title like "Favorite Sports of Students," label your X-axis ("Sport") and Y-axis ("Number of Students"), and pick colors that are easy to read.
6. **Review the Result** — Your finished chart should look something like this simple sketch:

```
Frequency or No. of Students
8 |
6 |        ###
4 |  ###   ###        ###
2 |  ###   ###   ###   ###
0 +------------------------------
    Cricket Football Hockey Badminton
```

**What just happened?** You transformed a plain table of numbers into a chart that instantly shows cricket is the clear favorite — something that would take a reader much longer to notice by scanning raw numbers alone.

> **REMEMBER:**
> 1. Google Sheets and Excel are easy tools for creating charts.
> 2. A dashboard shows multiple visuals in one place to tell a clear, complete data story.

### Interactive Stop-Point

**Pause & Think — 5.3:** Look at the bar chart you just built. If someone removed the axis labels and title entirely, could a stranger still understand what the chart is about? Why do labels matter just as much as the bars themselves?

### Quick Recap

Spreadsheet tools like Google Sheets and Excel let anyone — with zero coding experience — turn a plain table of numbers into a clear, shareable chart in just a few clicks.

---

## 5.4 Databases and Storing Data

### The Hook (Story Mode)

In 1970, a computer scientist at IBM named **Edgar F. Codd** was frustrated. Back then, computer data was often stored in messy, disorganized digital filing cabinets, where finding or connecting information was slow and painful. Codd proposed a radically cleaner idea: store data in structured **tables**, connected to each other through shared information, so a computer could instantly look up, update, or link records without confusion.

His idea became known as the **Relational Database** — and it is, quite literally, the invisible engine running underneath your bank account, your school's student records, Instagram's billions of photos, and almost every serious app you use today. You've been relying on Codd's 1970 idea, probably every single day, without ever knowing his name.

### The Explanation

After cleaning a messy survey table, we need to store that cleaned data in a proper format — either a spreadsheet or a database — so it stays organized, searchable, and ready for analysis. Let's explore how and where to store data.

There are two main ways to store structured data: (i) **Spreadsheets**, and (ii) **Databases**.

**Table 5.8: Spreadsheets vs Databases**

| Method | Description | Example Tool |
|---|---|---|
| **Spreadsheets** | A grid of rows and columns for small datasets | Excel, Google Sheets |
| **Databases** | A structured system to store and manage large data in tables | MySQL, SQLite |

> **TIDBIT:** Spreadsheets are good for small projects. Databases are better for big or multi-user data systems.

Here's an everyday way to picture the difference: **a spreadsheet is like a single notebook page** where you jot down your daily pocket money expenses — simple, personal, and easy to lose track of once it gets long. **A database is like an entire school's filing room**, with separate, connected folders for students, teachers, and grades — folders that can automatically stay in sync with each other, even when hundreds of people are using them at the same time.

**What is a Database?**

A **database** is an organized collection of data. It stores data in the form of tables. Each table is like a mini spreadsheet with rows and columns. Databases help in storing, retrieving, and updating data efficiently.

**Table 5.9: Database Terms — Meanings and Examples**

| Term | Meaning | Example |
|---|---|---|
| **Table** | A group of related data | Sports Survey |
| **Record** | A single entry (row) in the table | Ali's full row of data |
| **Field** | A specific piece of information (column) | Name, Sport, Frequency |

**DBMS and SQL**

A **Database Management System (DBMS)** is software used to create, manage, and interact with databases. Examples include MySQL, SQLite, and Microsoft Access.

To work with data inside a database, we use a language called **Structured Query Language (SQL)**. SQL lets us add, update, delete, or retrieve data using simple commands. Some basic SQL queries include:

- `SELECT * FROM Sports;` — This query shows *all* the data from the table named "Sports."
- `SELECT Name FROM Sports WHERE Favorite_Sport = 'Cricket';` — This query shows the names of students in the "Sports" table who like Cricket.
- `INSERT INTO Sports (Name, Favorite_Sport) VALUES ('Ali', 'Football');` — This query adds a brand-new entry to the table.

These basic SQL statements help manage and retrieve specific data from large databases quickly and efficiently — far faster than scrolling through a giant spreadsheet by hand.

### The Practical Walkthrough

Let's transform a messy paragraph of student information into a clean, structured database table, step by step.

**Messy paragraph:**

*"Ali is 15 years old and is in grade 10. Sara is 16 and in grade 10 too. Ahmad, who is 14, is in grade 9."*

1. **Identify the Entities** — Notice we're describing three separate students: Ali, Sara, and Ahmad. Each one will become its own **record** (row).
2. **Identify the Shared Attributes** — Every student has an ID, a Name, an Age, and a Grade. Each of these becomes a **field** (column).
3. **Create the Table Structure** — Set up column headers: `ID | Name | Age | Grade`.
4. **Fill In Each Record** — Carefully pull the correct value from the paragraph into each column, one student at a time.

**Resulting Database Table:**

```
+----+-------+-----+-------+
| ID | Name  | Age | Grade |
+----+-------+-----+-------+
| 1  | Ali   | 15  | 10    |
| 2  | Sara  | 16  | 10    |
| 3  | Ahmad | 14  | 9     |
+----+-------+-----+-------+
```

5. **Write a Simple Query** — Now that the data is structured, we can ask the database a question in SQL: `SELECT Name FROM Students WHERE Grade = 10;` This would return: **Ali, Sara**.

**What just happened?** You converted unstructured, hard-to-search paragraph text into a clean table that a computer can instantly search, filter, and update — the exact same transformation every real-world database performs on a much larger scale.

### Interactive Stop-Point

**Pause & Think — 5.4:** You are building a system for a hospital to store patient records. Why would it be incredibly risky to keep those records in a single, ordinary Excel spreadsheet instead of a secure, structured database?

### Quick Recap

Databases organize data into connected tables made of records (rows) and fields (columns), and SQL is the language we use to instantly search, retrieve, and update that data — even when it grows far too large for any spreadsheet to handle comfortably.

---

## Chapter Summary

- **Data Science** is the process of using data to understand problems, identify patterns, and make informed, smart decisions.
- **The Life Cycle (DSLC):** It follows a 6-step cycle: Problem Understanding, Data Collection, Cleaning/Validation, Analysis, Interpretation, and Visualization.
- **Data Collection:** Data is gathered from various sources like surveys (Google Forms), APIs, web scraping, and IoT sensors.
- **Data Quality:** Reliable data must be accurate, recent, and unbiased; diverse groups must be surveyed to avoid misleading results.
- **Cleaning & Validation:** "Messy" raw data must be cleaned by removing duplicates and fixing errors to ensure the results are trustworthy.
- **Data Visualization:** Charts turn complex numbers into easy-to-read visuals; Bar Charts compare groups, Pie Charts show parts of a whole, and Line Charts show trends over time.
- **SQL Language:** Structured Query Language (SQL) is used to communicate with databases using commands like SELECT (to get data) and INSERT (to add data).

---

## Multiple Choice Questions

1. What is the first step in the Data Science Life Cycle (DSLC)?
   (a) Collecting Data
   (b) Visualizing Data
   (c) Understanding the Problem
   (d) Analyzing the Data

2. Which method is best for collecting opinions from many students?
   (a) IoT Devices
   (b) Survey
   (c) Web Scraping
   (d) Database

3. What is "bias" in data?
   (a) Very large data size
   (b) Unfair or one-sided data
   (c) Well-cleaned data
   (d) High-speed data

4. Which tool is ideal for beginners to create charts?
   (a) Tableau
   (b) Python
   (c) Google Sheets
   (d) Hadoop

5. A relational database stores information in the form of:
   (a) Slides
   (b) Tables
   (c) Blocks
   (d) Layers

6. Which of the following charts is best for comparing groups?
   (a) Pie Chart
   (b) Bar Chart
   (c) Line Chart
   (d) Area Chart

7. What is the main goal of analyzing data?
   (a) Delete old data
   (b) Decorate data
   (c) Find patterns and make decisions
   (d) Upload to the internet

8. Which of the following tools is an advanced data visualization platform?
   (a) MS Paint
   (b) Google Data Studio
   (c) Notepad
   (d) WhatsApp

9. What should be done before storing data?
   (a) Add animations
   (b) Clean and validate it
   (c) Encrypt it
   (d) Translate it

10. Which one is an example of a data source?
    (a) YouTube
    (b) Survey form
    (c) Whiteboard
    (d) Slide show

## Short Questions

1. What is the importance of understanding a problem before collecting data?
2. Name any two methods of collecting data and give one example of each.
3. What do we mean by "cleaning" data?
4. Why is it important to validate data before using it?
5. What is the purpose of visualizing data using charts?
6. How does bias in data affect results?
7. Write two steps you will follow to clean a messy survey.
8. Name any two tools used for creating charts.

## Long Questions

1. Explain the six steps of the Data Science Life Cycle (DSLC) with one line each.
2. Give a detailed comparison between Bar Chart, Pie Chart, and Line Chart with examples.
3. Differentiate between DBMS and SQL.
4. Write a Query in SQL to get all data of a student whose roll_number is 15 from the student table.

## Answer Key for Multiple Choice Questions

1. (c) Understanding the Problem
2. (b) Survey
3. (b) Unfair or one-sided data
4. (c) Google Sheets
5. (b) Tables
6. (b) Bar Chart
7. (c) Find patterns and make decisions
8. (b) Google Data Studio
9. (b) Clean and validate it
10. (b) Survey form
