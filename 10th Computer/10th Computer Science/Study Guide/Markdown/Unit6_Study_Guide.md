# Unit 6: Introduction to Artificial Intelligence (AI) and Machine Learning (ML)

## Student Learning Outcomes

By the end of this chapter, you will be able to:

- Define artificial intelligence (AI) and machine learning (ML).
- Differentiate between AI and ML, understanding their unique characteristics and applications.
- Understand the concept of supervised learning and its application to teach systems to make predictions.
- Comprehend unsupervised learning, used for clustering and pattern recognition.
- Understand different algorithms and choose relevant algorithms based on specific business problems, including simple linear regression.
- Get familiar with key model performance metrics, especially accuracy.
- Understand where AI and ML are applied in daily life, business, and education.
- Discuss bias, privacy, and responsibility when using AI.

---

## Introduction

Let's start with a confession: every single one of you has already "used" artificial intelligence today. Maybe your phone unlocked because it recognized your face. Maybe YouTube guessed exactly what video you wanted next. Maybe you typed "he is comming" and your keyboard quietly fixed it to "he is coming" before you even noticed.

None of that is magic. It is math, wrapped in code, running on a computer that has seen a *lot* of examples.

That is the whole secret of this chapter, and honestly, the whole secret of AI. Once you know it, you can never "un-know" it — and you will start spotting AI and ML everywhere, from your mother's TikTok feed to the traffic signal at the end of your street.

In this chapter, you'll explore how computers use data to spot patterns, make predictions, and group similar things — kind of like your brain does, just faster, and without ever getting bored. By the end, you won't just know *what* AI and ML are. You'll know *how* to tell them apart, *where* they show up in Pakistan every day, and *why* we have to be careful with them.

Let's dig in.

---

## 6.1 AI, ML, and Overview

### The Hook (Story Mode)

In 1950, a British mathematician named Alan Turing asked a question that sounds almost too simple: *"Can machines think?"*

He knew that "thinking" is a slippery word — how do you even test it? So he designed a game, now called the **Turing Test**. A human judge chats through text with two hidden partners: one is a real person, one is a machine. If the judge cannot reliably tell which is which, the machine passes.

Turing never claimed a machine that passes his test is truly "thinking" the way you and I do. But he gave the world its first practical way to measure machine intelligence — and that single question, asked over 70 years ago, is the great-grandparent of every chatbot, voice assistant, and AI tool you use today.

### The Explanation

**6.1.1 What is AI?**

**Artificial Intelligence (AI)** is the ability of a machine or computer program to perform tasks that normally require human thinking and ability — things like understanding speech, recognizing images, or making decisions.

Notice what that definition does *not* say. It does not say the machine is conscious. It does not say the machine "understands" anything the way you do. It just says the machine can *perform* tasks that would otherwise need a human brain.

**Real-life examples (from Pakistan):**

- Urdu speech-to-text apps used in schools and educational institutes.
- Chatbots used by banks like **HBL** and **JazzCash** for customer support.
- Traffic control systems in big cities, such as the one run by the **Safe City Authority in Lahore**.

**6.1.2 What is ML?**

**Machine Learning (ML)** is a *part of* AI. It means training a machine to learn from data and make decisions on its own, without a programmer writing a specific instruction for every single situation.

**Definition:** ML is a method where computers learn from past data to predict or decide something.

**Examples:**

- Netflix or YouTube recommends videos based on your watch history.
- A weather app uses past temperatures to predict tomorrow's weather.

**6.1.3 Differences between AI and ML**

Here's the relationship in one sentence: **AI is the big goal. ML is one of the main tools we use to reach it.**

**The Hook for this section:** Think about your kitchen. An automatic microwave with a fixed "Popcorn" button always runs the exact same 3-minute timer, no matter what you put inside. That is **rule-based AI** — smart-*seeming*, but really just a fixed set of instructions written by a human. Now picture a smart oven that weighs the food, checks its moisture, and adjusts cooking time based on thousands of past cooking results. That oven is *learning* from data. That is **ML**.

**Table 6.1: Differences between AI and ML**

| Feature | AI | ML |
|---|---|---|
| **Definition** | Making machines smart enough to mimic human behavior | Teaching machines to learn from data and improve |
| **Main Goal** | To perform smart tasks like humans | To make predictions or decisions from data |
| **Needs Data?** | Sometimes (uses data to act smartly) | Always (needs data to learn) |
| **Like Human Behavior?** | Yes (like speaking, seeing, or understanding) | No (just learns patterns) |
| **Real-Life Example** | Chatbot on JazzCash that replies to customers | App that predicts electricity usage next week |

> **TIDBIT:** Think of AI as the brain, and ML as the experience that teaches the brain how to improve. AI is the broader concept of machines acting smart, while ML is when machines learn from data to make predictions or decisions.

### The Practical Walkthrough

Here's a simple way to decide, for *any* smart-seeming tool you meet, whether it's showing you AI in general or specifically ML:

1. **Ask: "Does it perform a human-like task?"** — If a machine can see, hear, speak, translate, or decide something, you're looking at **AI** (the umbrella term).
2. **Ask: "Did it get better by looking at data, or was it just told exact rules?"** — If a human programmer wrote every single rule by hand (e.g., "if button = popcorn, cook for 180 seconds"), it is **rule-based AI**, not ML.
3. **Ask: "Was it trained on examples?"** — If the system was shown thousands (or millions) of past examples — past emails, past photos, past prices — and it found the pattern *itself*, you're looking at **ML**.
4. **Conclude:** Every ML system is a type of AI. But not every AI system uses ML.

**What just happened?** You now have a 3-question checklist you can run on *any* "smart" gadget or app to sort it correctly — a skill most adults using these apps every day don't even have.

### Interactive Stop-Point

**Pause & Think — 6.1.1:** A traffic signal changes to green automatically every 60 seconds, no matter how many cars are waiting. A different traffic light uses cameras to watch the queues and clears the busiest lane first. Which one demonstrates true AI-like decision-making, and why? *(Hint: go back to the microwave vs. smart oven example.)*

### Quick Recap

AI is the broad goal of building machines that act smart. ML is the specific technique of teaching machines to learn that smartness from data instead of fixed rules.

---

## 6.2 Machine Learning Types

### The Hook (Story Mode)

In the late 1990s, the first email spam filters were fairly dumb — they blocked any email containing certain banned words. Spammers just misspelled the words ("V1AGRA") and slipped right through.

The real breakthrough came when early webmail services started letting *millions of users* click a "This is Spam" button. Suddenly, engineers had huge piles of email, each one labeled by a real human as either "Spam" or "Not Spam." Feed that labeled pile into a learning algorithm, and it starts finding its own patterns — patterns far more detailed than any human could hand-write as a rule. This is the origin story of **supervised learning** as we use it today.

### The Explanation

Just like students can learn with a teacher's guidance, or by exploring on their own, machines can learn in two main ways: **Supervised Learning** and **Unsupervised Learning**.

**6.2.1 Supervised Learning**

**The Hook:** Imagine studying math from a textbook that has an answer key in the back. You attempt a problem, guess an answer, flip to the back, check if you were right, and adjust your method next time. That repeated cycle of *guess → check → adjust* is exactly how supervised learning works.

**Definition:** Supervised learning is when the machine is trained using **labeled data** — data where both the input (the example) and the correct output (the answer) are provided.

**Example 1:** Suppose you are training a machine to tell an apple from a mango. You show it many pictures, each one labeled:
- "This is an Apple"
- "This is a Mango"

The computer studies these labeled examples. Later, when shown a *new*, unlabeled photo, it can predict — with high accuracy — whether it's an apple or a mango.

**Example 2:** A school system can be trained on past students' marks and attendance records (each one labeled "passed" or "failed") to predict which current students might be at risk of failing.

**6.2.2 Unsupervised Learning**

**The Hook:** Imagine you're handed a jumbled pile of coins from ten different countries, with no labels at all — no names, no values. You don't know what any of them are called. But you can still sort them into neat piles just by their shape, color, and size. Nobody told you the "correct" grouping — you found it yourself.

**Definition:** Unsupervised learning is when the machine finds patterns or groups in **unlabeled data**, without being told what the correct answer is.

**Example 1:** A store uses unsupervised learning to group customers by shopping habits, helping it market products better — even without knowing the "official" name for each customer type.

**Example 2:** A school wants to divide students into study groups. The system looks at their interests and subjects and forms groups based purely on similarity, without knowing which group is "best."

**6.2.3 Supervised vs Unsupervised Learning**

**Table 6.3: Supervised vs Unsupervised Learning**

| Feature | Supervised Learning | Unsupervised Learning |
|---|---|---|
| **Labeled Data?** | Yes (machine is told the correct answers) | No (machine finds patterns on its own) |
| **Main Task** | Predict or classify | Group or cluster similar data |
| **Example** | Predict student results using marks and study hours | Group customers based on shopping behavior |
| **Use in School** | Identify students who need help | Make automatic student groups for projects |

> **TIDBIT:** Think of Supervised Learning as learning with a teacher, and Unsupervised Learning as exploring on your own.

### The Practical Walkthrough

Let's trace exactly how a supervised learning classifier is trained to sort fruit images, step by step:

1. **Collect the Training Data** — Gather hundreds of fruit photos. This raw collection of examples is called the **dataset**.
2. **Label the Data** — A human tags each photo: "Apple" or "Mango." This is now a **Labeled Dataset** — a collection of inputs paired with the correct target answers.
3. **Feature Extraction** — The system notices measurable details in each photo: color, shape, size, texture. These measurable details are called **features**.
4. **Make a Prediction** — The system takes a *new* photo it hasn't seen before and guesses: "Apple" or "Mango," based on the patterns it found in the training features.
5. **Error Check** — The system compares its guess to the *actual* label (if we're still testing it) and measures how far off it was.
6. **Adjustment** — The system slightly tweaks its internal pattern-matching rules to reduce that error next time.
7. **Repeat** — Steps 4 through 6 happen thousands of times, across thousands of images, until the predictions become reliably accurate.

**What just happened?** You just traced the entire training loop of a real-world supervised learning system — the same basic loop (guess → check → adjust) used by apps that scan your face to unlock your phone.

Now let's do the same for an unsupervised clustering pipeline, grouping online shoppers by purchase history:

1. **Collect Unlabeled Data** — Gather each shopper's purchase history: what they bought, how often, how much they spent. No labels — nobody has tagged these shoppers as "type A" or "type B."
2. **Extract Features** — The system measures things like average spending, categories purchased, and frequency of orders.
3. **Measure Similarity** — The system compares shoppers to each other and calculates how "close" or "similar" their shopping patterns are.
4. **Form Clusters** — Shoppers with similar patterns are automatically grouped into clusters — say, "frequent small buyers" and "occasional big spenders" — even though no human wrote those group names in advance.
5. **Business Uses the Groups** — The store can now target each cluster with different offers, without ever knowing an "official" label for who these customers are.

**What just happened?** The machine created its own categories from patterns in the data — nobody told it what the categories should be.

### Interactive Stop-Point

**Pause & Think — 6.2.1:** You want to train an AI model to detect fake currency notes. What data would you need to provide for a *supervised* learning approach? Think carefully about what the "label" would be for each example.

**Grab a Partner — 6.2.3:** One partner describes a problem — for example, "grouping playlist songs by tempo" or "predicting house prices in Islamabad." The other partner identifies whether it needs Supervised or Unsupervised Learning, and names the inputs and, if applicable, the output.

### Quick Recap

Supervised learning uses labeled data to predict or classify — like studying with an answer key. Unsupervised learning uses unlabeled data to find hidden patterns and groupings — like sorting unknown coins by instinct.

---

## 6.3 Practical Applications of AI/ML

### The Hook (Story Mode)

Every time you say "Kal 8 bajay mujhe jagana" to Google Assistant in Urdu, a chain of AI systems fires into action almost instantly: one system converts your spoken Urdu into text, another understands *what you actually meant* (set an alarm, not just random words), and a third sets the alarm and replies to confirm. All of that happens using **speech recognition** and **natural language processing** — both powered by AI — in under two seconds.

### The Explanation

**6.3.1 Smart Assistants and Recommendations**

AI powers many of the tools that quietly make your day easier.

**Smart Assistants:** Tools like Google Assistant and Siri use AI to understand voice commands, translate languages, set reminders, and answer questions.

**Recommendation Systems:** These systems suggest what you might like, based on your past activity.

**Examples:**

- YouTube recommends videos after you watch a few clips.
- Daraz suggests clothes based on your browsing history.
- Instagram shows you videos similar to ones you've already watched.

These apps use **ML** specifically — not just AI in general — to analyze your habits and steadily improve their suggestions over time.

> **TIDBIT:** If the app makes suggestions, understands your voice, answers you, or learns your habits — it's very likely using AI and ML together.

**6.3.2 Business Use Cases Using Customer Analysis and Chatbots**

AI helps businesses understand customers, answer questions, and improve their services.

**Customer Analysis:** Companies collect data about customers to figure out which products sell best, to whom, and when.

*Example:* A grocery delivery app like **Cheetay** uses ML to suggest items you frequently buy, and to predict which items will be in demand in which city.

**Chatbots and Automated Help:** Many Pakistani banks, telecom companies, and e-commerce sites now use chatbots — smart systems that understand typed questions and respond automatically, without needing a human agent for every query.

AI helps businesses work faster, save money, and keep customers happy — all by harnessing the power of data.

**6.3.3 Bias, Privacy, and Responsibility**

While AI systems are powerful, they must be used responsibly. This is one of the most important ideas in this entire chapter, so let's slow down here.

**Bias in AI:** Sometimes machines learn *unfair* patterns from the data they're trained on. This is called **bias**. For example, if a speech-recognition system is trained mostly on English or male voices, it may perform poorly for Urdu speakers or female voices — not because it's "prejudiced" on purpose, but because its training data simply didn't include enough of those examples.

> **REMEMBER:** Always use diverse and balanced training data to reduce bias.

**Privacy and Data Use:** AI systems often use personal data — your name, your location, your choices — and that raises real privacy concerns. If an app tracks your movements or listens through your microphone without clear permission, that data can be misused.

**Best Practice:**

- Always ask for user permission before collecting data.
- Protect data using encryption.
- Never collect more data than is actually needed.

**Responsibility of Humans:** AI is *just a tool* — humans must use it wisely. If an AI-powered system makes a wrong decision, the responsibility lies with the humans who built or deployed it. For example, if a facial recognition system wrongly flags an innocent person, the humans running that system are responsible for catching the mistake and fixing it — not the algorithm itself.

Here's something worth remembering: even the biggest research labs in the world — teams with far more resources than any classroom — deal with bias and privacy mistakes constantly. Spotting a flaw in an AI system or a dataset is not a sign that something has gone "wrong" with your understanding. It's actually a core skill of a real computer scientist. If you can find the bias, you're already thinking like an engineer.

> **REMEMBER:** AI is used in smart assistants, shopping apps, and chatbots. Businesses use them for customer service and sales analysis. We must always consider ethics — fairness, privacy, and responsibility.

### The Practical Walkthrough

Here's a simple procedure for auditing *any* AI system for possible bias, something you can genuinely try on apps you use:

1. **Identify the Training Data Source** — Ask: what data was this system trained on? Whose voices, faces, or behaviors are represented?
2. **Identify Who's Missing** — Ask: which groups of people are likely *underrepresented* in that data — by language, gender, region, or income level?
3. **Predict the Weak Spot** — Based on step 2, predict where the system is most likely to perform poorly.
4. **Test It (if possible)** — Try the system yourself, or research reported cases, to see if your prediction was correct.
5. **Suggest a Fix** — Propose how the training data could be made more diverse and balanced to close that gap.

**What just happened?** You just performed a simplified version of the exact bias audit that real AI ethics teams run on production systems.

### Interactive Stop-Point

**Pause & Think — 6.3.3:** A hiring algorithm trained on ten years of a company's past hiring data starts rejecting qualified female applicants, even though no one programmed it to be sexist. Using the walkthrough above, what likely caused this bias in the training data — and what would you change to fix it?

### Quick Recap

AI and ML quietly power the assistants, recommendation feeds, and chatbots you use every day — but that same power means engineers must actively guard against bias, protect user privacy, and take responsibility for how these systems behave.

---

## 6.4 Supervised and Unsupervised Algorithms

### The Hook (Story Mode)

In the 1800s, a scientist named Francis Galton — long before computers existed — became fascinated by a strange question: could you predict how tall a child would grow, just from knowing the height of their parents? He plotted hundreds of parent-and-child height pairs on paper and noticed something striking: the points roughly followed a straight line. Taller parents tended to have taller children, and shorter parents tended to have shorter children — with a fairly predictable, straight-line relationship.

Galton had accidentally discovered what we now call **linear regression** — over a century before it became one of the most widely used tools in machine learning.

### The Explanation

Data science uses various algorithms to find patterns, make predictions, or analyze large amounts of data. Choosing the right algorithm depends on the type of data you have and the kind of problem you're trying to solve.

Some common algorithms include:

- **Linear Regression:** Predicts future values based on a straight-line relationship (e.g., predicting student scores from study hours).
- **Decision Trees:** Uses a tree-like model to make decisions based on yes/no questions (e.g., predicting if a customer will buy or not).
- **K-Means (Clustering):** Groups similar items together (e.g., grouping students with similar interests).

These algorithms help organizations solve real-world problems — predicting exam results, grouping customers for better marketing, and spotting patterns in fraud or health data.

> **TIDBIT:** Think of an algorithm like a recipe in the kitchen. It tells the computer what ingredients (data) to use and what steps to follow to get the final dish (a prediction or a group).

**6.4.1 Linear Regression**

**The Hook:** Imagine a teacher wants to predict how well students will perform on a test, based purely on how many hours each one studied. This is *exactly* Galton's height problem, just swapped from parents and children to study hours and test scores.

Simple linear regression predicts a value based on the relationship between two things:

- **Input (X):** Study hours
- **Output (Y):** Test score

Linear regression finds a straight line that best fits the data — a line you could use to predict a new student's score if you knew only their study hours.

**Table 6.5: Student Data**

| Study Hours (X) | Test Score (Y) |
|---|---|
| 1 | 35 |
| 2 | 45 |
| 3 | 50 |
| 5 | 55 |
| 6 | 65 |
| 8 | 70 |
| 9 | 75 |
| 10 | 80 |

If you plotted this data on a graph — Study Hours along the bottom, Test Scores up the side — you would see the dots trending steadily upward, and a straight "best-fit" line could be drawn right through the middle of them. If a student studied for 6.5 hours, you could read their predicted score straight off that line, even though 6.5 hours doesn't appear in the original table.

> **DO YOU KNOW?** Simple linear regression uses just one input to predict one outcome. But in real life, outcomes usually depend on many things. **Multiple linear regression** lets a computer consider several inputs at once — for example, predicting exam scores from study hours *and* attendance *and* sleep hours together — to improve prediction accuracy.

### The Practical Walkthrough

Let's calculate a basic linear regression prediction by hand, step by step, using the equation format $\text{Score} = (m \times \text{Study Hours}) + b$, where $m$ is the slope (how much the score rises per extra hour studied) and $b$ is the baseline score at zero hours.

1. **Look at the Data's Pattern** — From Table 6.5, notice test scores rise roughly 5 points for every extra hour studied, starting from around 30 points at zero hours.
2. **Write the Line's Formula** — A line that reasonably fits this data is: $\text{Score} = (5 \times \text{Study Hours}) + 30$.
3. **Understand Each Part** — The **slope (5)** tells you the score increases by about 5 points for every extra hour of study. The **baseline (30)** is the predicted score for a student who studied 0 hours — a starting point before any studying happens at all.
4. **Plug In a New Value** — Predict the score for a student who studied 6.5 hours: $\text{Score} = (5 \times 6.5) + 30 = 32.5 + 30 = 62.5$.
5. **Interpret the Result** — The model predicts this student would score approximately 62.5 out of 100.

**What just happened?** You just performed the core calculation behind every linear regression prediction — real ML systems use exactly this formula shape, just with slopes and baselines calculated automatically from much larger datasets.

### Interactive Stop-Point

**Pause & Think — 6.4.1:** Given the linear regression equation $\text{Score} = (10 \times \text{Study Hours}) + 20$, predict the exam score of a student who studied for 5 hours. What is the baseline score if study hours equal zero, and what does that baseline actually represent in real life?

### Quick Recap

Linear regression finds the best straight line through past data, letting us predict new outcomes — like test scores — from a known input, like study hours.

---

## 6.5 Evaluating Model Performance

### The Hook (Story Mode)

During World War II, engineers built some of the earliest radar systems to detect incoming enemy aircraft. But radar had a serious problem: flocks of birds sometimes produced signals that looked almost identical to airplanes. Radar operators had to constantly ask two questions: *"Did we correctly spot a real aircraft?"* and *"Did we mistake a flock of birds for an aircraft?"*

Every prediction any system makes — whether it's 1940s radar or a modern ML model — falls into one of these same kinds of categories: correctly right, correctly safe, or two different kinds of *wrong*. That is precisely what a confusion matrix measures.

### The Explanation

Once an ML model is trained — for example, to predict who will buy a product, or whether a message is spam — we need to measure how good it actually is. This helps us decide if the model is accurate and reliable enough to trust.

**6.5.1 Confusion Matrix**

A **confusion matrix** is a simple table showing how many predictions were correct or incorrect.

**Table 6.6: Confusion Matrix** (example: will a student pass or fail?)

| | Predicted: Pass | Predicted: Fail |
|---|---|---|
| **Actual: Pass** | True Positive (TP) | False Negative (FN) |
| **Actual: Fail** | False Positive (FP) | True Negative (TN) |

Let's define each box in plain words:

- **TP (True Positive):** The model predicted "pass," and the student actually passed. A correct prediction.
- **TN (True Negative):** The model predicted "fail," and the student actually failed. Also a correct prediction.
- **FP (False Positive):** The model predicted "pass," but the student actually failed. A false alarm.
- **FN (False Negative):** The model predicted "fail," but the student actually passed. A missed opportunity.

The confusion matrix helps us understand exactly *where* a model is making mistakes — and it lets us calculate one of the most important performance measures: **accuracy**.

**Accuracy:** Accuracy tells us how many predictions were correct, out of *all* predictions made.

$$\text{Accuracy} = \frac{TP + TN}{TP + TN + FP + FN}$$

### The Practical Walkthrough

Let's build a confusion matrix from scratch and calculate accuracy, step by step, using a class of 15 students where 8 actually passed and 7 actually failed.

1. **Gather the Raw Results** — Suppose the model produced these outcomes when checked against the real results:
   - Correctly predicted pass (TP) = 7
   - Correctly predicted fail (TN) = 5
   - Wrongly predicted pass (FP) = 2
   - Wrongly predicted fail (FN) = 1

2. **Place Each Number in the Matrix** — Fill Table 6.6's four boxes with these exact numbers: TP = 7, TN = 5, FP = 2, FN = 1.

   **What just happened?** You now have a complete visual snapshot of every correct and incorrect prediction the model made, sorted into four clear categories.

3. **Add Up the Correct Predictions** — $TP + TN = 7 + 5 = 12$. Out of 15 students, the model got 12 predictions right.

4. **Add Up All Predictions** — $TP + TN + FP + FN = 7 + 5 + 2 + 1 = 15$. This confirms our total matches the class size.

5. **Calculate Accuracy** — $\text{Accuracy} = \dfrac{12}{15} = 0.80$, or **80%**.

   **What just happened?** You calculated that this model is correct 80% of the time — a single, clear number that tells you how trustworthy the model is, straight from the confusion matrix.

6. **Look Beyond Accuracy** — Notice the model made 2 false positives (predicted "pass" for students who actually failed) and only 1 false negative. In a real classroom, which mistake is more costly — telling a struggling student they're fine (FP), or telling a passing student they need extra help (FN)? There's rarely one "correct" answer — it depends on what matters most in the situation.

### Interactive Stop-Point

**Grab a Partner — 6.5.1:** You're given raw predictions for 10 medical patients tested for a disease. Partner A counts the True Positives and False Positives from the results. Partner B counts the True Negatives and False Negatives. Together, fill in the full confusion matrix, calculate the accuracy, and discuss: for a disease test specifically, which error type — a False Positive or a False Negative — is more dangerous for patient health, and why?

### Quick Recap

A confusion matrix sorts every prediction into four categories — TP, TN, FP, and FN — and accuracy tells you, as one simple number, how often the model got it right overall.

---

## Chapter Summary

- **AI** enables machines to perform smart tasks. **ML**, a part of AI, allows machines to learn from data to make predictions or identify patterns, without being explicitly reprogrammed for every situation.
- **Supervised Learning** uses labeled data (e.g., predicting student grades or customer purchases).
- **Unsupervised Learning** uses unlabeled data (e.g., grouping people by preferences or behavior).
- **Linear Regression** predicts values along a straight-line relationship.
- **Decision Trees** make decisions through yes/no branching questions.
- **K-Means Clustering** finds natural groupings within data.
- A **Confusion Matrix** and **Accuracy** let us measure exactly how well a trained model performs.

---

## Multiple Choice Questions

1. What is Artificial Intelligence (AI)?
   (a) Solving math problems by hand
   (b) Machines performing tasks like humans
   (c) Sending emails using a computer
   (d) Watching videos online

2. Which of the following is an example of AI?
   (a) A chatbot replying to your questions
   (b) Using a whiteboard
   (c) A TV remote
   (d) Typing on a keyboard

3. What is Machine Learning (ML)?
   (a) Teaching humans to use machines
   (b) Teaching machines to learn from data like humans do
   (c) Learning computer hardware basics
   (d) A machine without internet

4. Which app recommends videos using ML?
   (a) Google Maps
   (b) Microsoft Paint
   (c) YouTube
   (d) Windows Media Player

5. In supervised learning, the data is:
   (a) Unorganized
   (b) Without any answers
   (c) Labeled with correct answers
   (d) Only text-based

6. Which of the following is an example of unsupervised learning?
   (a) Predicting student marks
   (b) Identifying spam emails
   (c) Marking quizzes
   (d) Grouping students by interest without labels

7. Google Assistant is an example of:
   (a) A game app
   (b) A word processor
   (c) A smart assistant using AI
   (d) A calculator

8. What skill is essential for a data analyst?
   (a) Painting
   (b) Basic drawing
   (c) Interpreting and visualizing data
   (d) Flying drones

9. AI is mostly used for:
   (a) Handwriting notes
   (b) Making phone calls
   (c) Charging phones
   (d) Smart decision making and automation

10. A chatbot on JazzCash is an example of:
    (a) Cloud computing
    (b) Data visualization
    (c) AI in business
    (d) Unsupervised learning

## Short Answer Questions

1. What is the difference between AI and ML?
2. Give one real-life example of AI used in Pakistan.
3. How does supervised learning work?
4. Define confusion matrix.
5. How can businesses use AI?
6. Give one example each of a smart assistant and a recommendation system.
7. What kind of data is used in unsupervised learning?

## Long Answer Questions

1. Explain supervised and unsupervised learning with suitable examples.
2. Explain how model performance is evaluated in machine learning using the following metrics:
   (a) Confusion Matrix
   (b) Accuracy
3. A model predicts if students will pass (1) or fail (0). Out of 20 students:
   - True Positives (TP) = 8
   - True Negatives (TN) = 6
   - False Positives (FP) = 4
   - False Negatives (FN) = 2

   You are required to (a) fill the confusion matrix, and (b) calculate accuracy.
