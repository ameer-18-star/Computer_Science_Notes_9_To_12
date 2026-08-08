# Chapter 7: Hypothesis Testing
### A Grade 12 Computer Science Study Guide

---

## Introduction: The Core Question

**The Hook.** In 1986, the space shuttle *Challenger* exploded 73 seconds after launch. Engineers had data showing that O-ring seals failed more often in cold weather. But nobody ran the numbers properly the night before launch. The temperature that morning was colder than any previous launch. Seven astronauts died. This is one of the most painful lessons in history about *why we must test our assumptions with data, not gut feeling.*

Now bring this closer to home. Imagine you are a software engineer. Your team just shipped a new AI code assistant. Everyone "feels" like it makes coding faster. But feelings are not proof. Maybe it's a coincidence. Maybe the team just got lucky this week. How do you know, with real confidence, that the improvement is *real* and not just random luck?

This is exactly the problem **hypothesis testing** solves. It is a mathematical toolkit that lets you say, with a measured amount of confidence: "Yes, this change really works," or "No, we don't have enough evidence yet."

Throughout this chapter, think of yourself as a **digital detective**. You collect evidence (data). You weigh that evidence mathematically. You reach a verdict. Let's begin.

---

## 7.1 Introduction to Hypothesis Testing

### The Hook (Story Mode): The Lady Tasting Tea

In 1935, a woman at a British research institute claimed she could tell, just by tasting, whether milk was poured into a cup before or after the tea. Most scientists in the room laughed it off. But statistician **Ronald Fisher** did not laugh. He designed a careful experiment: eight cups, four made one way and four the other, given to her in random order. Fisher then asked a sharper question: *if she were just guessing randomly, what is the probability she'd get this many right by pure luck?*

That single question — "could this just be luck?" — is the seed of everything you will learn in this chapter. Fisher's tea experiment became the foundation of modern hypothesis testing.

### The Explanation

**Meaning of a Hypothesis in Computer Science and Data Analysis**

A **hypothesis** is a clear, testable statement about something you believe might be true. In plain words: it's a guess you can check with data.

In computer science, hypotheses show up everywhere:
- "This new caching algorithm reduces average response time."
- "Users click more on Button Color A than Button Color B."
- "This new machine learning model has higher accuracy than the old one."

Notice: each of these can be *checked* by collecting data. That's what makes it a real hypothesis, not just an opinion.

**Transforming Research Questions into Testable Hypotheses**

A **research question** is the big question you want answered ("Does my new algorithm make searches faster?"). A hypothesis takes that fuzzy question and turns it into a sharp, measurable statement.

```
Research Question →  "Is our new database index faster?"
Hypothesis        →  "The average query time with the new index
                       is lower than the average query time with
                       the old index."
```

A good hypothesis has three properties:
1. **Clear** — no vague words like "better" without defining what "better" means.
2. **Measurable** — you can attach a number to it (time, accuracy %, click rate).
3. **Falsifiable** — it must be possible for the data to prove it wrong.

**Role of Hypothesis Testing in Modern Data Analysis and Software Engineering**

Hypothesis testing gives engineers and data scientists a disciplined way to answer: *"Is this result real, or did it happen by chance?"* Without it, teams risk shipping "improvements" that are actually just random noise. Companies like Google, Netflix, and Amazon run thousands of hypothesis tests every year (commonly called **A/B tests**) before rolling out changes to their products.

**Quick Recap:** A hypothesis is a testable guess, and hypothesis testing is the disciplined process of checking that guess with real data instead of gut feeling.

### Interactive Stop-Point — Pause & Think (7.1)

Your friend says: "I changed the font on my app, and now people use it more! My change worked!" 
- What is the *research question* here?
- Turn it into a clear, measurable hypothesis.
- What data would you need to collect to test it?

---

## 7.2 Types of Hypotheses

### The Hook (Story Mode): The Courtroom Trial

Picture a courtroom. The defendant is presumed **innocent until proven guilty**. The prosecutor must present overwhelming evidence to convict. This "innocent by default" position is exactly how statisticians think.

- **Null Hypothesis (H₀)** = "Innocent." The default assumption: no effect, no difference, nothing special happening.
- **Alternative Hypothesis (H₁ or Hₐ)** = "Guilty." The claim of change: something real is happening.

The jury (our statistical test) only convicts (rejects H₀) if the evidence is strong enough — "beyond reasonable doubt," which in statistics is our significance level.

### The Explanation

**Null Hypothesis (H₀): The "No Difference / Default Status Quo" Assumption**

H₀ always states that nothing has changed — no effect, no difference, no relationship. It is the boring, skeptical, "prove it to me" position we start from.

Example: *H₀: The new AI code assistant does not reduce coding time (average time is the same as before).*

**Alternative Hypothesis (H₁ or Hₐ): The "Claim of Change / Effect"**

H₁ is the opposite of H₀. It's the exciting claim — the one you often *hope* is true, but you must prove it with evidence.

Example: *H₁: The new AI code assistant reduces coding time (average time is lower than before).*

**Rules for Formulating Correct, Mathematically Sound Hypotheses**

1. H₀ and H₁ must cover all possibilities and never overlap.
2. Both must be written in terms of a measurable population parameter (a mean μ, a proportion p, a variance σ²).
3. Decide **before** collecting data whether your test is:
   - **Two-tailed**: H₁: μ ≠ μ₀ (just checking for *any* difference, in either direction)
   - **One-tailed**: H₁: μ > μ₀ or μ < μ₀ (checking for a difference in one specific direction)

```
Example — Two-tailed:
  H0: mu_A = mu_B     (no difference between A and B)
  H1: mu_A != mu_B    (there IS a difference, direction unknown)

Example — One-tailed:
  H0: mu_new <= mu_old   (new method is not better)
  H1: mu_new >  mu_old   (new method is genuinely better)
```

**Quick Recap:** H₀ is the skeptical default ("nothing changed"); H₁ is the claim you're trying to support with evidence. You never "prove" H₁ directly — you only gather enough evidence to reject H₀.

### Interactive Stop-Point — Pause & Think (7.2)

A software company claims: *"Our new AI code assistant reduces coding time."*
- Write the exact H₀ and H₁ for this claim, using proper mathematical notation.
- Is this a one-tailed or two-tailed test? Justify your choice.

---

## 7.3 Concepts in Hypothesis Testing

### The Hook (Story Mode): Student's t-Test at the Guinness Brewery

In 1908, a chemist named **William Sealy Gosset** worked at the Guinness brewery in Dublin, testing the quality of barley and beer using very small sample sizes. He developed a new statistical method to handle uncertainty from small samples. But Guinness had a strict rule: employees could not publish company secrets. So Gosset published his work under the pseudonym **"Student."** That's why one of the most widely used tools in this chapter — the **t-test** — is still called "Student's t-test" today.

### The Explanation

**Test Statistics (z, t, F, χ²): Measuring How Far Data Strays from the Null Assumption**

A **test statistic** is a single number, calculated from your sample data, that measures how far your observed result is from what H₀ predicted. A large test statistic means your data looks very different from H₀'s prediction.

| Test Statistic | When to Use It |
|---|---|
| **z** | Large samples, population standard deviation known |
| **t** | Small samples, population standard deviation unknown (most common in real engineering data) |
| **F** | Comparing variances between two or more groups |
| **χ² (Chi-Square)** | Comparing categorical / frequency data |

**t-value formula:**

```
        x̄ - μ
  t  =  -------
        s / √n

Where:
  x̄  = sample mean
  μ  = population mean assumed under H0
  s  = sample standard deviation
  n  = sample size
```

**Critical Region and Rejection Boundaries**

The **critical region** (or rejection region) is the zone of extreme values where, if your test statistic lands there, you reject H₀.

```
        Acceptance Region                 
  <-------------------------------->      
                                            
   Rejection |                | Rejection
   Region    |                | Region
  <----------|                |---------->
            -1.96      0     +1.96
       (for a two-tailed test at alpha = 0.05)
```

If your calculated t or z value falls beyond ±1.96 (for α = 0.05, two-tailed), it lands in the rejection region — meaning the result is unusual enough that we doubt H₀.

**Significance Level (α = 0.05): Defining the Threshold for Uncertainty**

The **significance level (α)** is the amount of risk you're willing to accept of wrongly rejecting a true H₀. α = 0.05 means: "I accept a 5% risk of a false alarm." It is chosen **before** running the test — never after seeing the results (choosing it afterward is a form of cheating called p-hacking, covered in 7.6).

**The p-value and Its Critical Importance**

The **p-value** is the probability of seeing a result as extreme as (or more extreme than) what you observed, *assuming H₀ is true.*

Everyday analogy: flip a coin 10 times and get 10 heads in a row. The p-value answers: "If this coin were perfectly fair, what's the probability of getting 10/10 heads by pure chance?" The answer is about 0.00097 — extremely unlikely. That tiny probability is strong evidence the coin (or our assumption) isn't what we thought.

**One-sentence summary:** The p-value tells us the probability that our results were just a lucky coincidence, while the significance level defines how much coincidence we are willing to accept before we stop believing it's a coincidence.

**Decision rule:**

```
   if p-value <= alpha:
       REJECT H0        (result is statistically significant)
   else:
       FAIL TO REJECT H0  (not enough evidence)
```

### Bridging Concept: Type I and Type II Errors

No test is perfect. There are two ways a decision can go wrong:

| | H₀ is actually True | H₀ is actually False |
|---|---|---|
| **We Reject H₀** | ❌ Type I Error (False Alarm) | ✅ Correct decision |
| **We Fail to Reject H₀** | ✅ Correct decision | ❌ Type II Error (Missed Effect) |

Analogy: **Type I Error** is like sending an innocent person to prison — you rejected "innocent" (H₀) when it was true. **Type II Error** is like letting a guilty person go free — you failed to reject "innocent" when it was actually false. In software testing, a Type I error is a "false positive bug alert" and a Type II error is a "real bug that slipped past testing."

### Bridging Concept: Confidence Intervals and Degrees of Freedom

A **confidence interval** gives a range of plausible values for the true population parameter, instead of just one number. A "95% confidence interval" means: if we repeated this experiment many times, 95% of the intervals we calculate would contain the true value.

**Degrees of freedom (df)** roughly means "how much independent information your sample has left after estimating something from it." For a simple one-sample t-test, df = n − 1 (you lose one degree of freedom because you used the sample to estimate the mean).

### The Practical Walkthrough: t-value Calculation

Suppose we sample 25 students with an average score of 80. We want to test whether this differs from the known population mean of 75. Sample standard deviation s = 10.

```
Step 1: State values
  x̄ = 80, μ = 75, s = 10, n = 25

Step 2: Apply formula
        80 - 75        5
  t  =  --------  =  ------  =  2.5
        10 / √25       2
```

A calculated t of 2.5 is compared against the critical t-value from the t-distribution table (with df = 24). If 2.5 exceeds the critical value, we reject H₀.

### Interactive Stop-Point — Grab a Partner (7.3)

Partner A runs 100 completely random statistical tests on pure noise data (no real pattern at all) until, purely by chance, one test returns p = 0.04. Partner A excitedly claims: "I found a real discovery!"

- Partner B: explain in your own words why this claim violates statistical ethics.
- What is this practice called (hint: see Section 7.6)?
- How many "significant" results would you *expect* to see by pure chance alone if you ran 100 tests at α = 0.05?

**Quick Recap:** The test statistic measures how far your data strays from H₀; the critical region and p-value tell you whether that distance is unusual enough to reject H₀ at your chosen significance level.

---

## 7.4 Performing Hypothesis Tests

### The Hook (Story Mode): Google's 41 Shades of Blue

In 2009, Google engineers couldn't agree on which shade of blue to use for search result links. Instead of guessing, they ran a live hypothesis test — showing **41 different shades of blue** to real users and measuring click-through rates. The winning shade wasn't just "prettier" — it was mathematically proven to generate about **$200 million more per year** in ad revenue. This is hypothesis testing at massive commercial scale.

### The Explanation: The 5 Standard Steps of Executing Any Hypothesis Test

```
  ┌─────────────────────────────┐
  │ 1. State H0 and H1           │
  └──────────────┬───────────────┘
                  ▼
  ┌─────────────────────────────┐
  │ 2. Choose Significance Level │
  │    (usually alpha = 0.05)    │
  └──────────────┬───────────────┘
                  ▼
  ┌─────────────────────────────┐
  │ 3. Collect Sample Data       │
  └──────────────┬───────────────┘
                  ▼
  ┌─────────────────────────────┐
  │ 4. Calculate Test Statistic  │
  │    and p-value               │
  └──────────────┬───────────────┘
                  ▼
  ┌─────────────────────────────┐
  │ 5. Compare p-value to alpha  │
  │    → Reject or Fail to Reject│
  └─────────────────────────────┘
```

### The Practical Walkthrough: A/B Test for Web Page Load Speed

**Scenario:** Your team built a new server-caching system. You want to know if it truly reduces average webpage load time (currently averaging 3.0 seconds).

**Step 1 — State Hypotheses**
```
H0: mu_new >= 3.0 seconds   (no real improvement)
H1: mu_new <  3.0 seconds   (genuinely faster)
```
(One-tailed test, since we specifically expect improvement.)

**Step 2 — Set Significance Level**
```
alpha = 0.05
```

**Step 3 — Collect Data**

Sample of 16 page loads with the new caching system gives:
```
x̄ = 2.6 seconds, s = 0.8 seconds, n = 16
```

**Step 4 — Calculate the Test Statistic**
```
        x̄ - μ         2.6 - 3.0        -0.4
  t  =  -------  =  --------------  =  -------  =  -2.0
        s / √n        0.8 / √16         0.2
```

**Step 5 — Compare to Critical Value / p-value**

For df = 15, one-tailed, α = 0.05, the critical t-value ≈ -1.753. Our calculated t = -2.0 is further into the rejection region (p-value ≈ 0.032, which is less than 0.05).

```
Decision:  p-value (0.032) < alpha (0.05)  →  REJECT H0
```

**What does this mean for our software system?** We have statistically significant evidence that the new caching system really does reduce load time — it's very unlikely this 2.6-second average happened by pure chance. It's reasonable to move forward with deployment (while still monitoring in production).

### Advanced Tests

**F-Test: Comparing Variances Between Algorithm Execution Times**

The **F-test** checks whether two groups have significantly different *variability* (not just different averages). This matters in engineering: an algorithm with a lower average time but wildly unpredictable spikes might be worse for a system that needs consistency.

```
        S1²
  F  =  -----
        S2²

Where S1² and S2² are the sample variances of Group 1 and Group 2.
```

**Example:** Two database indexing strategies are tested for query latency.
```
Strategy A variance = 16 ms²
Strategy B variance = 9 ms²

        16
  F  =  ---  =  1.78
         9
```
Compare F = 1.78 against the critical F-value from an F-distribution table (using each group's degrees of freedom). If 1.78 exceeds the critical value, the variances are significantly different — meaning one strategy is meaningfully less predictable than the other.

**Chi-Square (χ²) Test: Testing Independence and Goodness-of-Fit in Categorical Data**

The Chi-Square test checks whether *categorical* (bucketed/counted) data matches an expected pattern, or whether two categorical variables are related.

**Formula:**
```
        Σ (Oi - Ei)²
  χ² =  -------------
             Ei

Oi = Observed frequency in category i
Ei = Expected frequency in category i
```

**Walkthrough — Chi-Square Goodness-of-Fit Test on App Layout Clicks**

You test 4 app layout options with 200 total users, expecting an even 50 clicks each if layout truly doesn't matter (H₀: all layouts are equally popular).

| Layout | Observed (O) | Expected (E) | (O − E)² / E |
|---|---|---|---|
| A | 60 | 50 | 100/50 = 2.0 |
| B | 45 | 50 | 25/50 = 0.5 |
| C | 55 | 50 | 25/50 = 0.5 |
| D | 40 | 50 | 100/50 = 2.0 |
| **Total** | 200 | 200 | **χ² = 5.0** |

Compare χ² = 5.0 against the critical Chi-Square value at df = 3 (4 categories − 1), α = 0.05, which is about 7.815. Since 5.0 < 7.815, we **fail to reject H₀** — we don't have strong enough evidence that layout preference is unequal.

### Working Code Example (Python / SciPy)

```python
from scipy import stats
import numpy as np

# --- One-sample t-test example (page load speed) ---
sample = np.array([2.4, 2.7, 2.5, 2.9, 2.3, 2.8, 2.6, 2.5,
                    2.7, 2.4, 2.6, 2.5, 2.8, 2.6, 2.5, 2.6])
t_stat, p_value = stats.ttest_1samp(sample, popmean=3.0)
print("t-statistic:", t_stat)
print("p-value:", p_value / 2)  # divide by 2 for a one-tailed test

# --- F-test example (comparing two variances) ---
var_a, var_b = 16, 9
f_stat = var_a / var_b
print("F-statistic:", f_stat)

# --- Chi-Square goodness-of-fit test ---
observed = [60, 45, 55, 40]
expected = [50, 50, 50, 50]
chi2_stat, p_val = stats.chisquare(f_obs=observed, f_exp=expected)
print("Chi-square statistic:", chi2_stat)
print("p-value:", p_val)
```

### Interactive Stop-Point — Pause & Think (7.4)

A colleague ran an F-test and got F = 1.78, and says: "The variances are obviously different, look how much bigger 1.78 is than 1!" 
- Is this the correct way to interpret an F-test? What step is missing?

**Quick Recap:** Every hypothesis test follows the same 5 steps — state hypotheses, set alpha, collect data, calculate the statistic, and compare against your threshold. The F-test compares variability; the Chi-Square test compares categorical patterns.

---

## 7.5 Data Visualization For Hypothesis Testing

### The Hook (Story Mode): Seeing Before Believing

Before Fisher ever calculated a single p-value in the Lady Tasting Tea experiment, he could have simply looked at how many cups she got right. A quick visual — a bar showing 8/8 correct versus 4/8 expected by chance — tells a powerful story before the math even begins. Great data scientists *see* patterns before they *prove* them.

### The Explanation

**Importance of Data Visualization in Communicating Evidence**

Numbers alone are hard for people to absorb quickly. A well-designed chart lets both engineers and non-technical stakeholders instantly grasp whether a result looks meaningful — and visualization often reveals problems (outliers, skewed data) that raw numbers hide.

**Graphs and Charts for Presenting Results**

| Chart Type | Best Use |
|---|---|
| **Bar Chart** | Comparing averages across categories/groups (e.g., control vs. treatment) |
| **Box Plot** | Showing median, spread, and outliers — great for comparing variance |
| **Histogram** | Showing the full shape/distribution of a dataset |
| **Line Graph** | Showing trends and changes over time |
| **Scatter Plot** | Showing relationships between two continuous variables |

**ASCII Distribution View — Confidence Interval Overlap**

```
Group A:   [------|------]     mean = 2.6s
Group B:        [------|------]  mean = 3.0s
           2.2  2.6  3.0  3.4  (seconds)

If the intervals barely overlap or don't overlap at all,
that's a strong visual hint the difference may be real.
```

**Linking Data Visuals Directly with Accept/Reject Decisions**

A box plot comparing "Control Group" vs. "Treatment Group" response times can visually show almost no overlap — supporting a "Reject H₀" decision before you even see the p-value. Visuals and statistics should always tell the same story; if they disagree, double-check your work.

### Interactive Stop-Point — Pause & Think (7.5)

You are given a bar chart showing Group A's average score is slightly higher than Group B's. A classmate says: "The bars are different heights, so H₀ must be rejected!" 
- Why is this reasoning incomplete? What extra information (hint: variability, sample size, p-value) is needed before making that claim?

**Quick Recap:** Visualization helps you *see* evidence quickly and communicate it clearly, but the final accept/reject decision must always be backed by the actual statistical test — not just how a chart looks.

---

## 7.6 Ethical Issues in Data Science and Analysis

### The Hook (Story Mode): The Challenger Disaster, Revisited

Engineers at NASA's contractor had O-ring failure data from previous cold-weather launches. But when presenting to decision-makers the night before the Challenger launch, the data was poorly visualized and the statistical risk wasn't communicated clearly. The launch went ahead. This tragedy is a permanent reminder: **how you collect, analyze, and communicate data is an ethical responsibility, not just a technical one.**

### The Explanation

**Bias in Data Collection and Sampling Errors**

Bias happens when your data doesn't fairly represent the real population you're studying.

1. **Survey Bias** — surveying only top-performing schools about student performance.
2. **Sampling Bias** — a health study using only young adults, ignoring older people.
3. **Gender Bias** — a hiring dataset with mostly male candidates, causing a model to favor men.
4. **Geographical Bias** — using only urban data to make decisions for rural populations.
5. **Confirmation Bias** — a researcher only looking at data that supports what they already believe.

**Ethical Use of Data and Predictive Models (p-hacking, Data Dredging)**

**p-hacking** means running many tests, tweaking data, or trying different variables until you accidentally find a "significant" p-value — then reporting only that one result as if it were the plan all along. **Data dredging** is a related practice: digging through a large dataset looking for *any* pattern, without a real hypothesis stated in advance.

Why is this dangerous? Remember: at α = 0.05, about 1 in 20 tests will show "significance" purely by random chance, even with meaningless data. If you run 100 tests on noise and only report the 5 that "worked," you are lying with statistics — even if every individual calculation was done correctly.

**How to prevent p-hacking:**
- Decide your hypothesis and α **before** collecting data.
- Report *all* tests you ran, not just the significant ones.
- Use corrections (like the Bonferroni correction) when running multiple tests.
- Replicate significant findings with a fresh, independent dataset.

**Responsible Communication of Findings without Misleading Stakeholders**

- Never exaggerate a small effect as a "huge breakthrough."
- Always disclose the sample size, the test used, and the limitations of your data.
- Avoid visual tricks (truncated bar-chart axes, cherry-picked time windows) that make small differences look dramatic.

### Interactive Stop-Point — Grab a Partner (7.6)

Partner A: You're a data analyst under pressure to show your company's new app update is a "success." You ran 20 different tests on different app metrics; only one showed p = 0.048. Your manager wants you to write a report only about that one metric. 

Partner B: Write a short, ethical response explaining what you should actually report, and why.

**Quick Recap:** Ethical data science means collecting representative data, being transparent about every test you ran (not just the "winning" one), and communicating results honestly — because misleading data has caused real, tragic consequences.

---

## 7.7 Communicating Results and Conclusions

### The Hook (Story Mode): "Failing to Reject" Is Not "Proving"

Imagine a jury says "not guilty." That doesn't mean the defendant is proven innocent beyond all doubt — it means the prosecution didn't provide *enough* evidence to convict. In the exact same way, when a hypothesis test gives us a large p-value, we say **"fail to reject H₀"** — never **"H₀ is proven true."** There might simply not have been enough data yet to detect a real effect.

### The Explanation

**Interpreting Test Results Correctly (Failing to Reject vs. "Proving" H₀)**

| Correct Language | Incorrect Language |
|---|---|
| "We reject H₀ at the 0.05 level." | "We proved H₁ is true." |
| "We fail to reject H₀; insufficient evidence of an effect." | "We proved there is no effect." |
| "The data is consistent with H₀." | "H₀ is 100% confirmed." |

Statistics never *proves* anything with 100% certainty — it only measures how consistent your data is with a hypothesis, given a stated risk level (α).

**Presenting Technical Findings Clearly to Non-Technical Audiences**

- Lead with the plain-English conclusion, then support it with the numbers.
- Use visuals (from 7.5) to make the story intuitive.
- Avoid jargon like "we reject the null" without explaining what that means in real terms (e.g., "the new system really is faster, and it's very unlikely this happened by chance").
- State limitations honestly (sample size, possible bias, confidence level).

**Connecting Final Conclusions Back to Original Business/Research Hypotheses**

Always loop back to the original question. If the research question was "Is our new caching system faster?", your final conclusion should directly restate and answer that — not drift into unrelated observations.

```
Research Question → Hypothesis → Test → p-value → Decision → 
                     Conclusion (in plain English, tied back
                     to the original question)
```

### Interactive Stop-Point — Pause & Think (7.7)

Why is saying **"We proved the Null Hypothesis is 100% true"** technically incorrect in statistics? What should we say instead?

**Quick Recap:** Never claim a hypothesis test "proves" anything with certainty — always speak in terms of evidence, confidence, and risk levels, and always tie your conclusion back to the original research question.

---

## Chapter Summary Table

| Term | Plain-English Meaning |
|---|---|
| **Hypothesis** | A testable, measurable guess about data |
| **Hypothesis Testing** | A method to decide if sample evidence supports or rejects a claim |
| **Null Hypothesis (H₀)** | The default "no effect / no difference" assumption |
| **Alternative Hypothesis (H₁/Hₐ)** | The claim that there IS an effect or difference |
| **Test Statistic** | A number (z, t, F, χ²) measuring how far data strays from H₀ |
| **Critical Region** | The zone of extreme values where H₀ is rejected |
| **Significance Level (α)** | The risk of a false alarm you're willing to accept (commonly 0.05) |
| **p-value** | Probability of your result (or more extreme) occurring if H₀ were true |
| **Decision Rule** | If p-value ≤ α → reject H₀; otherwise → fail to reject H₀ |
| **Type I Error** | False alarm — rejecting a true H₀ |
| **Type II Error** | Missed effect — failing to reject a false H₀ |
| **F-Test** | Compares variances between two groups |
| **Chi-Square Test** | Compares observed vs. expected categorical frequencies |
| **Data Visualization** | Using graphs/charts to clarify and support test results |
| **Bias** | Unfair or unrepresentative data leading to misleading conclusions |
| **p-hacking** | Manipulating tests/data until a "significant" result appears by chance |
| **Ethical Use of Data** | Collecting, analyzing, and reporting data honestly and responsibly |

---

## End-of-Chapter Exercises

### Multiple Choice Questions

1. A hypothesis is:
   (a) A final result (b) A test value (c) A proposed explanation (d) A dataset

2. The null hypothesis represents:
   (a) An alternative idea (b) No effect or no difference (c) A final conclusion (d) A prediction model

3. The symbol used for the null hypothesis is:
   (a) H₁ (b) H₂ (c) H₀ (d) Hₐ

4. A p-value is used for:
   (a) Measuring accuracy (b) Testing a hypothesis (c) Measuring variance (d) Data storage

5. If p-value < α, the decision is to:
   (a) Accept H₀ (b) Reject H₀ (c) Ignore data (d) Recalculate the mean

6. The critical region is the:
   (a) Safe area (b) Rejection area (c) Data range (d) Sample space

7. An example of a test statistic is:
   (a) Mean (b) t-value (c) Mode (d) Median

8. Data visualization is used to:
   (a) Store data (b) Present results clearly (c) Delete data (d) Calculate the mean

9. A chart useful for comparison is:
   (a) Pie chart (b) Bar chart (c) Table (d) Text

10. Bias in data means:
    (a) Correct data (b) Balanced data (c) Unfair representation (d) Random data

**Answer Key:** 1-c, 2-b, 3-c, 4-b, 5-b, 6-b, 7-b, 8-b, 9-b, 10-c

### Short Questions
1. What is a hypothesis?
2. What is a research question?
3. Define the null hypothesis (H₀).
4. What is a test statistic?
5. What is meant by a p-value?
6. What is a critical region?
7. What are the basic steps in hypothesis testing?
8. Why is data visualization important?
9. What is bias in data collection?
10. Why is ethical use of data important?
11. What is the difference between a Type I error and a Type II error?
12. Why is "failing to reject H₀" different from "proving H₀"?

### Long Questions
1. Explain the concept of hypothesis testing and its role in data analysis and software engineering.
2. Describe different types of hypotheses and explain how to formulate correct, testable hypotheses.
3. Explain key concepts in hypothesis testing, including test statistics, critical region, significance level, and p-value.
4. Discuss the 5 steps involved in performing a hypothesis test, using a suitable computer science example (e.g., an A/B test).
5. Explain the F-test and Chi-Square test with worked examples, and describe when each should be used.
6. Explain the importance of data visualization in hypothesis testing and how graphs help present and support results.
7. Discuss ethical issues in data science, including bias, p-hacking, and responsible communication of findings.
8. Explain how to interpret hypothesis testing results correctly and connect conclusions back to the original hypotheses.

---

*End of Chapter 7: Hypothesis Testing*
