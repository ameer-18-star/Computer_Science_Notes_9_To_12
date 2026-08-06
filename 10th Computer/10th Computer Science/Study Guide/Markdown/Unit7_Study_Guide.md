# Unit 7: Applications of AI

### 10th Class Computer Science — A Student's Field Guide to Artificial Intelligence

---

## Welcome, Tech Investigator

Before we start, let's get one thing straight: you already use Artificial Intelligence every single day. When you search something on your phone, when a video app suggests your next watch, when you unlock your phone with your face — that's AI, quietly working behind the scenes.

This chapter is not about memorizing definitions. It's about becoming a **tech investigator** — someone who can open up any AI system, ask "how does this actually work?", and also ask the harder question: "is this fair?"

By the end of this unit, you will be able to:

- Explain how AI powers real tools like chatbots, robots, and voice assistants.
- Try out AI products yourself and reflect on how they work.
- Weigh the benefits and the limits of these tools honestly.
- Spot moments where AI has treated people unfairly.
- Think critically about how to fix those moments.
- Explain AI's social impact clearly, in writing and out loud.
- Carry ethical awareness into anything you build in the future.

No prior knowledge of AI is assumed anywhere in this chapter. Every technical word is explained in plain English the moment it shows up. Let's begin.

---

## Introduction

Computer Science is not just about using computers — it is about **solving problems**, **building smart tools**, and **making life easier**. One of the most exciting branches of modern Computer Science is **Artificial Intelligence (AI)**.

**Natural Language Processing (NLP)** helps computers understand human language — this powers chatbots, translation apps, and text tools. **Speech technology** powers voice assistants like Alexa and Google Assistant. **Recommendation systems** suggest videos, music, or products based on what you like. **Autonomous vehicles** — self-driving cars — use AI to move safely without a driver. **Robotics** shows up in factories, hospitals, and even space missions.

But AI is not magic, and it is not automatically fair. AI must be used carefully, so it does not harm people or create **social injustices** — situations where a system treats one group of people worse than another. Some AI systems show **bias** (unfair favoritism or unfair disadvantage toward a group) if they are not designed carefully. That is why anyone who builds or uses AI — including you — needs to understand data privacy, accountability, and ethical rules.

This chapter will help you think critically about AI: to recognize its benefits, understand its risks, and see how it touches jobs, education, health, and society as a whole.

---

## 7.1 Introduction to Artificial Intelligence (AI)

### The Hook (Story Mode)

In 1950, a British mathematician named **Alan Turing** asked a question that was way ahead of his time: *"Can machines think?"*

At that point, computers were room-sized machines that could barely do arithmetic. Turing didn't have an answer to his own question, so instead, he designed a clever test. In what we now call the **Turing Test**, a human judge has text conversations with two hidden participants — one human, one machine. If the judge cannot reliably tell which one is the machine, the machine passes the test.

Notice what Turing did here: he didn't try to define "thinking." He built a **test** for it instead. That single idea — judge intelligence by behavior, not by what's happening inside — quietly became one of the founding ideas of Artificial Intelligence.

### The Explanation

**Artificial Intelligence (AI)** is a field of computer science that teaches machines to "think" and "act" in ways that resemble human intelligence. AI helps computers:

- Solve problems
- Learn from data (information fed into a computer)
- Make smart decisions — **without being told every single step**

That last point is the real difference between AI and a normal computer program. A calculator app follows a fixed rule every time: 2 + 2 always equals 4 because a programmer typed that rule in directly. An AI system, by contrast, is often *shown* thousands of examples and learns the pattern on its own.

AI already shows up in:

| Area | Everyday Example |
|---|---|
| Mobile Apps | Face unlock, predictive text |
| Online Shopping | "You might also like…" suggestions |
| Health Care | AI helping doctors spot diseases in scans |
| Transportation | Maps predicting the fastest route |

When you talk to a voice assistant or chat with a website's chatbot, you are using AI directly. It helps doctors detect disease, helps drivers navigate roads, and helps students find answers online.

> **Did You Know?** AI can now write stories, solve math problems, and even create art — just like a human can.

**Plain-language definition to remember:**
> *"Artificial Intelligence is computer software that learns from data to perform tasks that normally require human intelligence."*

### The Practical Walkthrough — "Spot the AI" Investigation

1. **Pick a device.** Grab your phone, or think of one your family uses.
2. **Open three different apps** — for example, a maps app, a shopping app, and a video app.
3. **For each app, ask:** "Is this app deciding something *for* me, based on data about me?" (A route suggestion, a product suggestion, a video suggestion.)
4. **Write one sentence per app** describing what data you think it used to make that decision (your location, your past purchases, your watch history).
5. **What just happened?** You just performed your first "AI audit" — identifying where automatic decision-making is quietly working in the background of ordinary apps.

### Interactive Stop-Point

**Pause & Think:** Think of one task in your own daily life that a computer already does *without* being told every single step (for example, your phone predicting the next word you're about to type). What data do you think it uses to make that guess?

### Quick Recap

AI is software that learns patterns from data instead of following one fixed instruction, and it already sits quietly inside apps you use every day.

---

### 7.1.1 Impact of AI on Jobs and Work

### The Hook (Story Mode)

A hundred years ago, if you wanted to make a phone call, a **human telephone switchboard operator** had to physically plug your line into the right socket to connect you to the person you were calling. Entire buildings were staffed with rows of operators doing this all day.

Then automatic switching systems arrived. The switchboard operator job faded away almost completely. But here's the twist: it didn't destroy the telephone industry — it *transformed* it. New jobs appeared: telecom engineers, network technicians, call-center software designers. The repetitive task disappeared; new, more complex roles took its place.

### The Explanation

AI is changing the way people work, in a very similar pattern. In factories, robots and AI-powered machines now do jobs that were once done only by human workers — often faster, for longer hours, and with fewer mistakes.

At the same time, AI is **creating new kinds of jobs**. Someone has to design, train, test, and manage these AI systems. That's why roles like:

- **Data Scientist** — someone who studies data to find patterns
- **AI Developer** — someone who builds AI-powered software
- **Machine Learning Engineer** — someone who builds and trains AI models

...are among the fastest-growing careers in the world today.

**Simple way to remember it:** AI doesn't just delete jobs — it usually **replaces repetitive tasks** and **creates new, more technical roles** at the same time.

### The Practical Walkthrough — "Before and After AI" Chart

1. **Draw two columns** on a page: "Before AI" and "After AI."
2. **Pick a familiar industry** — for example, banking, retail, or transportation.
3. **List 2–3 jobs or tasks** that used to be done entirely by humans in that industry (example: bank tellers counting cash by hand).
4. **In the "After AI" column, write what changed** (example: ATMs and mobile banking apps now handle routine transactions, while human staff focus on advice and complex problems).
5. **What just happened?** You just mapped how automation *shifts* labor rather than simply erasing it — a much more accurate picture than "robots will take all the jobs."

### Interactive Stop-Point

**Pause & Think:** Name three jobs that might change significantly due to AI in the next 10 years. What new skills will workers need to adapt?

### Quick Recap

AI often replaces repetitive manual tasks, but it simultaneously opens up new technical careers — the challenge for workers is adapting their skills, not simply competing against machines.

---

## 7.2 Data and AI

### The Hook (Story Mode)

Think about how you personally got better at recognizing your neighbors' faces. You didn't read a rulebook describing exact eye-spacing and nose shape. You simply **saw them many times**, in different lighting, from different angles, and your brain quietly built a pattern.

AI systems learn almost the same way — except instead of "seeing your neighbor," they are shown huge piles of examples called **data**.

### The Explanation

**Data** is information — numbers, words, images, sounds — that gets fed into a computer. Data is the single most important ingredient in AI. AI learns from data the way a student learns by reading books: the more relevant material it studies, and the more accurate that material is, the smarter it becomes.

When an AI system receives large amounts of information from many different sources, it can find **patterns** — repeating relationships in the data — and use those patterns to make better decisions.

> **Did You Know?** An AI trained with poor-quality data can give wrong answers or make unfair decisions.

**Plain-language definition to remember:**
> *"Data is the raw information an AI system studies in order to learn a pattern."*

### Quick Recap

AI is only as good as the data it learns from — good data in, good decisions out; bad data in, bad decisions out.

---

### 7.2.1 Automatic Data Collection

### The Hook (Story Mode)

Picture a smart wristwatch on your arm right now. As you walk to school, it silently counts your steps. As you sleep, it silently tracks your heart rate and sleep cycle. You never typed a single number into it — the watch just *collected* all of that on its own.

### The Explanation

**Automatic data collection** means gathering information without a person typing it in by hand. Many everyday devices and apps do this constantly:

| Device/App | Data Collected Automatically |
|---|---|
| Mobile Phone | Location, app usage, search history |
| Shopping Website | Clicks, product views, time spent per page |
| Fitness Watch | Steps, heart rate, sleep patterns |

With automatic collection, AI systems can adjust and respond to user needs almost instantly. This saves time, reduces human error, and allows systems to run without needing a person to feed them information constantly.

### The Practical Walkthrough — "What Data Do Apps Collect?" Survey

1. **Open the settings** of 2–3 apps on a phone (with permission from a parent or guardian).
2. **Look for a "Permissions" or "Privacy" section.**
3. **Note down what each app is allowed to access** — location, microphone, contacts, photos.
4. **For each permission, ask:** "Why would this app need this information to work well?"
5. **What just happened?** You just traced the invisible pipeline of automatic data collection that most people scroll past without ever reading.

### Interactive Stop-Point

**Grab a Partner:** One partner names an app; the other guesses three types of data it probably collects automatically, and explains why the app would need each one.

### Quick Recap

Automatic data collection lets devices gather information constantly and silently, which is what allows AI systems to respond to us quickly — but it also means we should always know *what* is being collected and *why*.

---

### 7.2.2 Types of Data: Quality and Quantity

### The Hook (Story Mode)

Imagine training a dog to recognize cats using **only pictures of white cats**. The dog gets really good at spotting white cats. But the very first time it sees a brown cat, it has no idea what it's looking at — because its "training set" never included one. The dog wasn't dumb; its *training data* was incomplete.

### The Explanation

In AI, two properties of data matter enormously:

- **Quantity** — how much data is available. If a system studies many different examples, it becomes familiar with many different situations.
- **Quality** — how correct and useful the data is. If the data contains mistakes, missing values, or confusing labels, the AI can learn the wrong lessons entirely.

| Feature | Good Quality Data | Poor Quality Data |
|---|---|---|
| Labels | Clear and correct | Missing or wrong |
| Coverage | Represents many groups/situations | Represents only one group |
| Errors | Very few mistakes | Many mistakes or typos |
| Result | Reliable AI decisions | Confused, unfair AI decisions |

> **Did You Know?** AI learns best with both ingredients together: big (quantity) *and* accurate (quality).

### The Practical Walkthrough — Spotting Dataset Problems

1. **Look at a sample dataset** described to you (for example: "1,000 photos of cats, but 950 of them are the same three white cats photographed repeatedly").
2. **Check the sample size.** Is 1,000 actually a large *variety*, or just a large *repetition*?
3. **Check the representation.** Are different breeds, colors, and settings included?
4. **Predict the outcome.** Based on the gaps you found, predict what kind of cat the AI would likely misidentify.
5. **What just happened?** You just performed a mini "data quality audit" — the exact first step any responsible AI developer takes before training a model.

### Interactive Stop-Point

**Grab a Partner:** Partner A suggests training an AI image scanner using 10,000 low-quality photos. Partner B suggests using 100 high-quality photos. Discuss: which model will perform better, and why?

### Quick Recap

Quantity gives an AI system broad experience, but quality determines whether that experience is trustworthy — a system needs both to make fair, accurate decisions.

---

## 7.3 Real-World Applications of AI

AI is now used across daily life — in businesses, schools, hospitals, and homes — helping things run smarter and faster. Let's walk through five major applications one at a time.

---

### 7.3.1 Natural Language Processing (NLP)

### The Hook (Story Mode)

In 1966, a computer scientist at MIT named **Joseph Weizenbaum** built a program called **ELIZA** — one of the very first chatbots in history. ELIZA was designed to imitate a psychotherapist. It didn't actually "understand" language at all; it simply looked for keywords in what you typed and echoed them back as questions.

Type "I am sad about my mother," and ELIZA might reply, "Tell me more about your mother." Simple pattern-matching — yet many users at the time swore they were talking to something that truly understood them. ELIZA proved something important: language processing, even a very simple version of it, can feel remarkably human.

### The Explanation

**Natural Language Processing (NLP)** is the part of AI that helps computers understand human language. It allows machines to read text, listen to speech, and reply in ways people can understand.

When you type a question into a search bar, or speak to a voice assistant, NLP is the layer that interprets what you meant and generates a sensible reply. In customer service, NLP-powered chatbots answer common questions without needing a human agent.

> **Tidbit:** Chatbots on websites can answer your questions 24/7, all thanks to NLP.

### The Practical Walkthrough — Tracing an NLP Pipeline

Let's trace exactly what (conceptually) happens when someone types: **"I love this camera!"**

1. **Tokenization** — the plain-language phase where the sentence gets broken into individual pieces: `["I", "love", "this", "camera", "!"]`.
   *What just happened?* The AI turned one long sentence into small, separately analyzable pieces.
2. **Understanding Structure** — the AI identifies which word is the subject ("I"), which is the action ("love"), and which is the object ("this camera").
   *What just happened?* The AI built a rough map of who is doing what to what.
3. **Sentiment Detection** — the AI compares words like "love" against a huge internal reference of words associated with positive or negative feeling.
   *What just happened?* "Love" is flagged as strongly positive, so the sentence is classified as **positive sentiment**.
4. **Output** — the system might respond with something like: "Glad you're enjoying the camera! Would you like to leave a review?"
   *What just happened?* The AI turned raw text into a useful, human-understandable action.

### Interactive Stop-Point

**Pause & Think:** How does a voice assistant distinguish between the words "there," "their," and "they're" — which all sound identical? What extra context clues must the NLP model look at?

### Quick Recap

NLP breaks language down into pieces a computer can analyze, then uses patterns in those pieces to understand meaning and generate a sensible response.

---

### 7.3.2 Robotics in Everyday Life

### The Hook (Story Mode)

In 1961, General Motors installed something new on its car assembly line: **Unimate**, the world's first industrial robot. Unimate's job was to lift and stack red-hot metal die-castings — a task that was exhausting and genuinely dangerous for human workers due to heat and heavy lifting. Unimate didn't get tired, didn't get burned, and worked with tireless precision. It quietly opened the door to an entire industry of industrial robotics.

### The Explanation

**Robotics** is the branch of AI involving machines — **robots** — built to physically perform tasks that resemble human actions. Robots can lift heavy items, assist in surgeries, or clean floors intelligently. They can assist elderly or disabled people with simple daily tasks. Because robots don't get tired and can work with great precision, they're especially valuable for repeated or dangerous work.

> **Did You Know?** Robots are now used in some restaurants to serve food and clean tables.

### The Practical Walkthrough — Analyzing a Robot's Task

1. **Watch (or picture) a robot performing a task** — for example, a robotic arm assembling a phone on a factory line.
2. **Identify the sensors it likely uses** — cameras (to see part positions), pressure sensors (to grip correctly without crushing parts).
3. **Identify the decision it's making** — "Is this part correctly aligned before I attach it?"
4. **Consider the failure case** — what happens if a camera misreads a part's position?
5. **What just happened?** You just broke a robot's "smart" behavior down into sensing, deciding, and acting — the three-step loop nearly every robot follows.

### Interactive Stop-Point

**Grab a Partner:** One partner describes a household chore. The other partner designs, out loud, what sensors and decisions a robot would need to complete that chore safely.

### Quick Recap

Robots combine sensors (to observe the world) with AI decision-making (to decide what to do next), which is why they excel at repetitive or dangerous tasks that would tire or endanger a human.

---

### 7.3.3 Speech Technology and Voice Control

### The Hook (Story Mode)

Picture yourself asking your smartphone out loud: *"What's the weather tomorrow?"* In under two seconds, your phone converts your voice into digital text, sends a request, processes an answer, and speaks it back to you — all without you touching the screen once.

### The Explanation

**Speech technology** is a type of AI that allows computers to listen to and understand spoken words. It helps machines turn voice into text, and then respond with a spoken answer. Voice assistants on phones or smart speakers are the clearest example.

Real-world uses include:

- **Customer service:** answering calls and guiding users without a human operator
- **Smart homes:** controlling lights or devices just by speaking
- **Healthcare:** helping doctors record notes without typing

> **Tidbit:** Smartphones can now unlock using your voice — no touching required.
> **Did You Know?** Some cars now respond to voice commands to turn on music, make calls, or give directions.

### The Practical Walkthrough — "Speak and See" Practice

1. **Open a voice-to-text tool** (like Google Voice Typing) on a phone or computer.
2. **Speak a clear sentence** and watch what text appears.
3. **Speak the same sentence again, but faster or in a different tone.**
4. **Compare the two results** — did the tool make different mistakes each time?
5. **What just happened?** You just discovered, hands-on, that speech AI accuracy depends heavily on clarity, speed, and pronunciation — exactly the kind of limitation engineers work to reduce.

### Interactive Stop-Point

**Pause & Think:** If a voice assistant kept mishearing a student's accent, what would that suggest about the training data used to build the tool?

### Quick Recap

Speech technology converts spoken sound into text and back again, making hands-free interaction possible — but its accuracy depends heavily on how varied and representative its training data was.

---

### 7.3.4 Recommendation Systems

### The Hook (Story Mode)

In 1998, Amazon introduced something called **Item-to-Item Collaborative Filtering** — a method of studying millions of customers' purchase patterns to predict what a *particular* shopper might want next. Instead of showing every customer the same "Top Sellers" list, Amazon could now say, essentially, "People who bought what you just bought also tended to buy this." It completely reshaped how online shopping — and later, streaming — worked.

### The Explanation

**Recommendation systems** are a part of AI that suggest content based on your past behavior — what you've viewed, searched, or selected. The system studies your patterns, compares them to patterns from other users, and shows you similar options.

For example, if you look at school bags on a shopping site, the AI may suggest other bags or related items. On an education platform, it might suggest videos related to what you've studied recently.

> **Tidbit:** When YouTube shows you "Videos you may like," that's AI learning your interests.

Recommendation systems make content more personal and useful — but they must be used carefully, so they don't invade privacy or trap users in a narrow bubble of repeated content.

### The Practical Walkthrough — Mapping a Recommendation Pipeline

Let's trace how a video app might decide what to recommend you next:

1. **User Action** — you just finished watching a cooking video.
   *What just happened?* The system logged this single action as a new data point about you.
2. **Pattern Matching** — the AI compares your action to millions of other users who also watched that same cooking video.
   *What just happened?* The AI found a "neighborhood" of users with similar tastes to yours.
3. **Filtering** — the AI checks what *those* similar users tended to watch next, and removes videos you've already seen.
   *What just happened?* The list of possible suggestions shrinks down to relevant, unseen options.
4. **Top 3 Predictions** — the AI ranks the remaining options and shows you its top three guesses.
   *What just happened?* You now see a personalized recommendation list — built entirely from pattern-matching, with no human manually choosing your suggestions.

### Interactive Stop-Point

**Grab a Partner:** One partner acts as a streaming app user who only watches sci-fi movies. The other acts as the recommendation engine, selecting three new movies to display. Explain your choices out loud.

### Quick Recap

Recommendation systems study your past behavior, compare it to similar users, and predict what you're likely to want next — powerful for convenience, but something that must respect privacy and avoid narrowing your options too much.

---

### 7.3.5 Autonomous Vehicles (Self-Driving Vehicles)

### The Hook (Story Mode)

Think about everything a human driver does without even thinking twice: eyes scanning the road, ears listening for horns, hands adjusting the wheel, a brain reacting in a split second to a pedestrian stepping off the curb. Now imagine replacing every one of those human senses and reflexes with a machine equivalent — cameras instead of eyes, microphones instead of ears, and an AI system instead of a brain making the split-second call.

### The Explanation

**Autonomous vehicles**, also called self-driving vehicles, are vehicles that can move on the road without a human driver. They use AI to understand their surroundings and make decisions on their own.

**Sensor map of a self-driving car:**

| Sensor | What It Detects |
|---|---|
| Cameras | Traffic lights, road signs, lane markings |
| Radar | Distance and speed of nearby vehicles |
| LiDAR / Proximity Sensors | 3D shape of nearby objects, even in the dark |
| GPS (Global Positioning System) | The car's exact location on a map |

Using these tools together with AI, the car can safely speed up, slow down, turn, or stop when needed. Benefits include:

- Fewer accidents caused by human error like distraction or tiredness
- Independence for people who cannot drive themselves, such as the elderly or disabled

Challenges include:

- Vehicles must be tested extensively to be safe in *all* conditions, not just ideal ones
- Concerns about job loss for professional drivers
- Unclear responsibility: who is at fault if a self-driving car causes an accident?

That is why engineers, governments, and companies must work together to build stronger safety testing and fairer traffic laws for AI-driven vehicles.

### The Practical Walkthrough — "Map the Journey" Planning Task

1. **Sketch a simple route** — for example, from your home to a nearby market.
2. **Mark every hazard point** along the route: a crosswalk, a traffic light, a sharp turn, a school zone.
3. **For each hazard point, list which sensor** (camera, radar, LiDAR, GPS) the car would rely on most.
4. **Identify one "hard case"** — a moment where multiple sensors would need to agree before the car acts (example: a pedestrian partially hidden behind a parked truck).
5. **What just happened?** You just built a simplified version of the sensor-fusion planning that real self-driving car engineers do before a vehicle ever touches a real road.

### Interactive Stop-Point

**Pause & Think:** An autonomous car faces an unavoidable obstacle in severe weather. What sensor data must it prioritize to make a safe, split-second stopping decision?

### Quick Recap

Self-driving cars replace human senses and reflexes with sensors and AI decision-making, offering major safety and accessibility benefits — but only if they are tested thoroughly and supported by clear, fair rules.

---

## 7.4 Benefits and Challenges of AI Applications

### The Explanation

AI applications help people complete tasks faster and more easily. In offices, AI systems manage files and answer routine questions. In education, AI can guide students through smart learning apps that adjust to their level. This frees up time for people to focus on more important decisions. AI also supports businesses in planning, predicting sales, and improving customer service — reducing human error and increasing efficiency across fields like agriculture, banking, and transport.

### Quick Recap

AI's biggest strength is speed and consistency at repetitive tasks — freeing humans to focus on judgment-heavy work.

---

### 7.4.1 Limitations and Challenges of AI Applications

### The Hook (Story Mode)

Imagine asking a chatbot a question written with a typo or unusual slang. It might completely misread your intent and give a strange, unrelated answer. That's not the chatbot being "silly" — it's a direct, traceable result of the language patterns it was trained on.

### The Explanation

AI systems are not always correct, and they can give wrong results, especially when trained on low-quality or biased data. A chatbot might misunderstand a question if the language is unclear. In fields like law or health, even small AI mistakes can cause serious problems — which is why careful testing is essential.

Other key challenges:

- AI can replace human workers in fields like customer service, data entry, and clerical work — leading to potential job loss.
- Many AI systems cannot make fair decisions if they are not designed carefully.

> **Did You Know?** AI systems can make mistakes if they are trained on incomplete or biased data.

### Interactive Stop-Point

**Pause & Think:** If you found out a customer-service chatbot kept giving wrong answers to a specific type of question, what would you check *first* — the code, or the training data? Why?

### Quick Recap

AI mistakes are never mysterious accidents — they are traceable to the data, code, or design choices humans made, which means they are also fixable by humans.

---

## 7.5 Ethics, Fairness, and Social Impact of AI

### The Explanation

**Ethics** in AI means using AI in a way that is fair, honest, and safe for everyone. Because AI can make real decisions that affect real people, it's critical that those decisions don't hurt anyone or treat any group unfairly. If an AI system gives better service to one group and ignores another, that is not fair — and it's not acceptable. AI should be developed with fairness, safety, and respect for human rights built in from the start.

> **Tidbit:** AI can be unfair if not designed properly — that's why developers must think carefully about what's right and wrong.

### Quick Recap

Ethics in AI isn't an optional add-on — it's a core design requirement, because the decisions AI makes have real consequences for real people.

---

### 7.5.1 Bias in AI and Algorithms

### The Hook (Story Mode)

Automatic soap dispensers use infrared sensors to detect a hand underneath and release soap. In several documented cases, these dispensers failed to work for people with dark skin — because the sensors were calibrated and tested almost entirely using light-skinned hands. The engineers weren't necessarily being deliberately unfair; their **testing data simply didn't represent everyone**. But the impact on the people left out was very real.

### The Explanation

**Bias** in AI happens when a system produces unfair results because of the data it was trained on. If the training data represents mostly one group of people, the AI may fail to understand or treat other groups fairly.

**Example:** a face recognition tool might not work well for all skin tones if it was trained mostly on images of one skin type. This shows that training data needs to include different people, languages, and situations. Removing bias is a critical step toward making AI genuinely fair and helpful for everyone.

**Biased vs. Fair AI Design — Facial Recognition Example**

| | Biased/Risky Implementation | Fair/Ethical Implementation |
|---|---|---|
| Training Data | 90% one skin tone, tested on employees at one office | Balanced across skin tones, ages, genders, and lighting conditions |
| Testing | Only tested internally, by the developer team | Tested externally by diverse volunteer groups before launch |
| Outcome | Fails frequently for underrepresented users | Performs consistently across all user groups |
| Accountability | No process to report failures | Clear feedback channel and regular bias audits |

### The Practical Walkthrough — Conducting a Mini Bias Audit

1. **State the AI's purpose** — for example, "This system unlocks a building door using face recognition."
2. **Ask who was in the training data.** Were different ages, genders, and skin tones represented?
3. **Ask who tested the system before launch.** Was it tested only by the developer team, or by a broader, diverse group?
4. **Predict the failure group.** Based on any gaps found, predict which group of users is most likely to be misidentified or denied access.
5. **Propose one fix.** Suggest one concrete change to the training data or testing process that would close the gap.
6. **What just happened?** You just completed the same core process — checking representation, checking testing, predicting harm, proposing a fix — that real AI ethics teams use before shipping a product.

### Interactive Stop-Point

**Pause & Think:** A facial recognition system used for building security is trained on data containing 90% male photos. What problem will occur when female employees try to enter?

### Quick Recap

Bias isn't a mysterious flaw — it's a direct, traceable result of unrepresentative training data, and spotting it is a genuinely valuable skill.

---

### 7.5.2 Fairness and Transparency in AI

### The Explanation

**Fairness** in AI means the system treats all users equally, regardless of race, gender, age, or background. This matters enormously in systems that make high-stakes decisions — like school admissions, job interviews, or legal cases. To ensure fairness, AI must be trained on data that represents all relevant groups and situations.

**Transparency** means people should be able to understand *how* an AI system works and *why* it reached a particular decision. If an AI rejects a loan application or selects a student for a program, the affected person has the right to know what rules or steps the system followed. Transparency helps catch mistakes early and builds public confidence that the system is being run honestly.

| | Low Transparency | High Transparency |
|---|---|---|
| Loan rejected | User told only "Application denied" | User told the specific factors that led to denial |
| Student not selected | No explanation given | Selection criteria shared clearly in advance |

### The Practical Walkthrough — AI Ethics Audit: School Admissions

1. **Describe the decision** — "An AI system ranks student applications for a limited number of program seats."
2. **List the factors it likely uses** — grades, attendance, extracurricular activities, an entrance test score.
3. **Check for fairness gaps** — could any of these factors disadvantage students from under-resourced schools who had fewer opportunities to build extracurricular records?
4. **Check for transparency** — are rejected students told *why* they weren't selected?
5. **Propose an improvement** — for example, adding a written explanation for every decision, or reviewing borderline cases with a human.
6. **What just happened?** You just performed a full AI ethics audit — the same structured thinking used by real institutions evaluating automated decision systems.

### Interactive Stop-Point

**"Explain Your Choice" Role Play:** One student plays "the AI" and is asked to select a classmate for a prize based on given criteria (attendance, grades, participation). The "AI" must explain, out loud, exactly which criteria led to the choice — practicing transparency in real time.

### Quick Recap

Fairness ensures AI treats everyone equally; transparency ensures people can understand and challenge AI decisions that affect them — both are essential, not optional, features of trustworthy AI.

---

### 7.5.3 Privacy, Data Security, and Surveillance

### The Explanation

**Privacy** means keeping personal information safe and not sharing it without permission. Many AI systems collect data such as names, addresses, location, or search history. If this data isn't protected, it can be stolen or misused.

**Data security** means protecting information from hackers, viruses, or other attacks. AI systems must use strong security methods to keep user data safe.

**Surveillance** is when systems or cameras watch people's actions. It can genuinely help with safety — but constant, unexplained monitoring can also harm people's sense of freedom and privacy. The line between "helpful safety tool" and "invasive surveillance" often comes down to **consent**, **purpose**, and **oversight**.

### Interactive Stop-Point

**Grab a Partner:** Debate public surveillance cameras equipped with AI facial recognition. One partner argues for the safety benefits; the other raises privacy concerns. Try to reach one shared recommendation by the end.

### Quick Recap

Privacy, security, and surveillance are three connected ideas: privacy is about *what's* collected, security is about *protecting* it, and surveillance is about *how* watching is used — and each needs its own careful limits.

---

### 7.5.4 AI and Social Equity (Fairness in Society)

### The Explanation

AI should help all people equally — including the poor, disabled, and those living in remote areas. Sometimes, new technologies like AI become available only to wealthier or more educated groups first, while others are left behind. This creates a widening gap between people who benefit from AI and people who don't.

To support fairness in society, AI tools should be designed so that everyone can benefit — not just a select few.

### Interactive Stop-Point

**Pause & Think:** Name one AI-powered tool that could genuinely help someone in a remote village (for example, AI-assisted medical diagnosis where no specialist doctor is nearby). What barrier might still stop them from accessing it?

### Quick Recap

Genuine fairness in AI isn't just about the algorithm being unbiased — it's also about making sure the technology actually *reaches* everyone who needs it.

---

## 7.6 Responsibility of AI Designers

### The Explanation

AI systems do not invent their own rules — they follow instructions built by human designers. This means the people who build AI carry real responsibility for making sure their systems are fair, safe, and helpful. If an AI system makes a wrong or unfair decision, the root cause is almost always traceable back to a design choice.

That's why AI designers must carefully consider how their tools will affect real people's lives. Building trustworthy AI isn't just a technical job — it's a **moral duty**.

> **Did You Know?** AI is only as good as the people who build it — which is exactly why designers must act responsibly.

### The Practical Walkthrough — "Build a Fair System" Brainstorm

1. **Choose a system to design** — for example, an AI tool for school admissions.
2. **List the data it would need.** Be specific: grades, attendance, extracurriculars, entrance test scores.
3. **List one rule to avoid bias.** For example: "Do not use the applicant's neighborhood as a factor, since it may correlate unfairly with income level."
4. **List one rule to ensure transparency.** For example: "Every rejected applicant receives a written explanation of the top three factors in the decision."
5. **List one rule for accountability.** For example: "A human reviewer checks any decision the AI is less than 70% confident about."
6. **What just happened?** You just built a basic ethical framework — the same kind of checklist real organizations use before deploying an AI system that affects people's lives.

### Interactive Stop-Point

**Pause & Think:** You are designing an AI application for medical diagnosis. What three ethical guidelines will you follow to ensure patient safety and fairness?

### Quick Recap

Every AI decision traces back to a human design choice — which means every AI mistake is also a human responsibility to fix.

---

### 7.6.1 Following Ethics in AI

### The Explanation

Ethics in AI means doing what is right and fair when creating or using AI systems. Designers must ensure their systems do not hurt people, spread false information, or treat anyone unfairly. Ethics guides designers toward decisions that protect users and support justice.

Following ethics also means being **honest about how the system works** — users should know what data is being used and how decisions are made. Ethical design is what builds real trust between people and technology.

### Interactive Stop-Point

**"Right or Wrong?" Ethics Quiz (try these out loud with a partner):**

1. An AI system secretly records conversations in a smart speaker without telling the user. *Right or wrong?*
2. An AI hiring tool explains clearly to every rejected applicant which skills they were missing. *Right or wrong?*
3. A recommendation app is designed to keep users scrolling as long as possible, even if it affects their sleep. *Right or wrong?*

For each one, explain your reasoning — there often isn't one single "correct" answer, and that's exactly the kind of judgment real AI ethicists wrestle with daily.

### Quick Recap

Ethical AI design means building honesty, fairness, and accountability directly into a system — not adding them as an afterthought once something goes wrong.

---

## Try It Yourself: Hands-On Activities

**Activity (NLP):** Type a sentence in English into Google Translate or a translation app, and convert it into Urdu. Then change a few words and try again. Notice what changes and what stays the same in the translation.

**Activity (Robotics):** Watch a short video of a robot performing a task (assembling parts, serving food, or cleaning). Write 3 lines about: what the robot did, how AI helped it, and what would happen if it made a mistake.

**Activity (Speech Recognition):** Use voice typing on a phone or computer (e.g., Google Docs voice typing). Speak a sentence and watch the text appear. Then speak a different sentence and check if the text is correct.

---

## Chapter Summary

- **AI** is a field of computer science that teaches machines to "think" and "act" like humans — solving problems, learning from data, and making decisions without step-by-step instructions.
- **Real-world applications of AI** include mobile apps, online shopping, healthcare, transportation, and voice assistants.
- **Impact on jobs:** AI replaces some repetitive jobs (like factory tasks) but creates new ones (AI developers, data scientists).
- **Data** is the essential fuel of AI — both **quantity** (how much) and **quality** (how correct) matter enormously.
- **NLP** helps computers understand and respond to human language.
- **Robotics** lets machines perform physical tasks — often repeated or dangerous ones.
- **Speech technology** turns voice into text and back into speech.
- **Recommendation systems** predict what you want based on patterns in past behavior.
- **Autonomous vehicles** use sensors (cameras, radar, LiDAR, GPS) and AI to drive without a human — reducing accidents and helping people who can't drive.
- **Bias** happens when unfair or incomplete training data leads to unfair outcomes.
- **Fairness** means equal treatment for all users, regardless of background.
- **Transparency** means people can understand and question how an AI decision was made.
- **Privacy, security, and surveillance** must be balanced carefully whenever AI systems collect personal data.
- **AI designers carry real responsibility** — every AI mistake traces back to a human design choice, and every fix starts there too.

---

## Exercise

### Multiple Choice Questions

1. What does AI stand for?
   A) Automatic Intelligence B) Artificial Intelligence C) Active Interface D) Applied Information

2. Which of the following is an example of Natural Language Processing (NLP)?
   A) Online calculator B) Voice typing C) File copying D) Image editing

3. What type of data helps AI make better decisions?
   A) Short and weak data B) Only images C) Large and good quality data D) Data without labels

4. Which tool uses AI to understand human voice?
   A) Video player B) Translator C) Speech recognition D) Mouse

5. What is the role of robots in factories?
   A) Watching videos B) Making websites C) Doing repeated or dangerous tasks D) Writing stories

6. What is a challenge of using AI?
   A) It works slowly B) It cannot be turned off C) It may replace human jobs D) It cannot store data

7. What is bias in AI?
   A) A computer error B) Equal results for everyone C) Unfair results due to bad data D) Fast performance

8. Why is fairness important in AI?
   A) So the system looks good B) To avoid slow speed C) To give equal treatment to all users D) To use more memory

9. Which of these is NOT an AI tool?
   A) Chatbot B) Face detection C) Spell checker D) Paper notebook

### Short Questions

1. What is Artificial Intelligence (AI)?
2. How is AI used in daily life?
3. Why does AI need large and good-quality data?
4. What is the role of Natural Language Processing (NLP)?
5. Give one example of robotics in everyday life.
6. What is the purpose of speech recognition technology?
7. How do recommendation systems work?
8. What is meant by bias in AI systems?
9. Why should AI systems be transparent and fair?

### Long Questions

1. What is the importance of data in AI? Explain why good and large data is needed.
2. Write in detail about any three real-world applications of AI (such as NLP, robotics, or speech technology).
3. Explain the ethical issues in AI. Why are fairness, privacy, and transparency important?

---

*End of Unit 7: Applications of AI*
