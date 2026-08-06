# UNIT 7: Emerging Technologies in Computer Science

---

> **"The best way to predict the future is to invent it."**
> — Alan Kay, Computer Scientist

---

## Student Learning Outcomes

By the end of this chapter, you will be able to:

- Define **Artificial Intelligence (AI)** in plain, simple words
- Identify AI applications in healthcare, education, gaming, finance, and more
- Explain AI subfields: Machine Learning, Deep Learning, NLP, Computer Vision, and Robotics
- Distinguish between **Whitebox (Explainable)** and **Blackbox (Unexplainable)** AI algorithms
- Define the **Internet of Things (IoT)** and explain why it matters
- Describe the key components of an IoT system: sensors, actuators, devices, networks, and data analysis
- Explore IoT applications in smart homes, healthcare, and transportation
- Discuss **security and privacy** challenges in IoT
- Think critically about the ethical challenges that come with AI and IoT

---

## Introduction

### 🎬 Story Mode: The Day Your City Woke Up

Imagine you are walking to school one morning. The streetlights turn off automatically as the sun rises. The traffic signal ahead turns green just as your school bus arrives — it "saw" the bus coming. Your smart water bottle reminds you to drink water. Inside your classroom, the air conditioner adjusts to the right temperature without anyone touching it.

None of this is magic. None of this requires a human to press a button.

This is the world of **Artificial Intelligence (AI)** and the **Internet of Things (IoT)** — two technologies that are quietly, powerfully changing everything around us.

In this chapter, you will not just learn definitions. You will understand *how* these technologies work, *where* they are already being used, and — most importantly — *how someone like you* could one day build them.

Let's begin.

---

## 7.1 Introduction to Artificial Intelligence (AI)

### 🎬 Story Mode: The First "Thinking" Machine

The year is **1955**. Two scientists, **Allen Newell** and **Herbert A. Simon**, sit in a lab at Carnegie Mellon University. They have a wild idea: *Can a computer solve problems the way a human brain does?*

They write a program called the **Logic Theorist**. It is the very first AI program in history. It can prove mathematical theorems — problems that usually require human reasoning. The world is amazed.

Fast forward to today. AI can diagnose diseases, drive cars, beat world champions at chess, and write poetry. But at its heart, the goal is still the same: **make machines think like humans**.

---

### What Is Artificial Intelligence?

**Artificial Intelligence (AI)** means giving a computer the ability to **think, learn, and make decisions** — the way a human does.

Think of it this way:

- A regular calculator can add 2 + 2 and give you 4. But it cannot *learn* from mistakes. It cannot *improve* over time.
- An AI system, on the other hand, can look at thousands of X-ray images, *learn* what a tumour looks like, and then *identify* tumours in new images — without a doctor telling it what to do each time.

> **In one sentence:** AI is the science of making computers smart enough to do tasks that normally need a human brain.

---

### 7.1.1 Applications of AI in Different Domains

AI is not just one technology in one place. It is everywhere. Let's explore where it is already changing lives.

---

#### 🏥 Healthcare

AI is helping doctors save lives.

- It analyses **medical images** (like X-rays and MRI scans) to detect diseases early
- It **predicts** which patients might get sicker before it happens
- It **personalises** treatment plans — figuring out which medicine works best for *this specific patient*

> **Real Example:** In Pakistan, AI-assisted robotic systems are being used to perform precise medical operations that reduce human error.

---

#### 🎓 Education

AI is making learning more personal.

- It tracks **how a student is learning** and adjusts difficulty accordingly
- It **automates** routine tasks like marking attendance or grading multiple-choice tests
- AI tutoring tools can explain concepts in different ways until the student understands

---

#### 🎮 Gaming

AI makes games feel alive.

- Enemy characters in video games **think** and **react** — they are controlled by AI
- AI can **generate entire game worlds** automatically
- It studies your playing style and **adapts** the game to challenge you better

---

#### 🚗 Transportation & Automobiles

AI is on the road.

- **Self-driving cars** use AI to see the road, understand traffic rules, and drive safely
- **Advanced Driver Assistance Systems (ADAS)** warn drivers about dangers
- AI **optimises fuel efficiency** and predicts when a car needs maintenance before it breaks down

---

#### 💰 Finance

AI is managing money.

- It **detects fraud** — if your bank card is used in an unusual way, AI flags it instantly
- It makes **personalised investment recommendations**
- It performs **algorithmic trading** — buying and selling stocks in milliseconds based on patterns

---

#### 📱 Social Media

AI decides what you see.

- The **"For You" feed** on TikTok, Instagram Reels, or YouTube is powered entirely by AI
- AI analyses what you like, watch, and share — then **predicts** what you will want to see next
- It also detects and removes harmful content automatically

---

#### 🌾 Agriculture

AI is helping farmers.

- **Sensors and cameras** scan crops to detect diseases or pest attacks early
- AI predicts **crop yields** based on weather, soil, and historical data
- **Automated irrigation systems** water only the areas that actually need it — saving water

---

#### 🛒 E-Commerce

AI is your personal shopping assistant.

- When you open an app like Daraz or Amazon, the **product recommendations** are AI
- **Chatbots** answer your customer service questions instantly — 24/7
- AI **detects fraudulent orders** and protects shoppers

---

### 📊 Visual Summary: AI Domains at a Glance

```
┌─────────────────────────────────────────────────────┐
│               ARTIFICIAL INTELLIGENCE               │
│                                                     │
│  Healthcare   Education   Gaming   Transportation   │
│     🏥           🎓         🎮          🚗           │
│                                                     │
│  Finance    Social Media   Agriculture   E-Commerce │
│     💰          📱            🌾            🛒       │
└─────────────────────────────────────────────────────┘
```

---

### ✋ Pause & Think #1

> Look at the list of AI domains above. Pick **one domain** that you use or see every day. Write down:
> 1. What task does the AI do?
> 2. What would happen if the AI made a mistake in that domain?
> 3. Is this AI application helpful, harmful, or both? Why?

Discuss with a partner. There is no wrong answer here — thinking critically is the goal.

---

### 7.1.2 Subfields of AI

AI is a huge field. Scientists have divided it into **smaller areas of focus**, each solving a different type of problem.

---

#### 🤖 Machine Learning (ML)

**Machine Learning** is a type of AI where computers **learn from experience**.

Instead of a programmer writing every rule, the computer is shown **thousands of examples** and it figures out the patterns on its own.

> **Analogy:** Imagine you are learning to recognise cats. At first, someone shows you photos of cats and says, "Cat. Not a cat. Cat. Cat. Not a cat." After seeing enough examples, you can identify a cat in any photo — even one you have never seen before. Machine learning works exactly like this.

**How it works (Step by Step):**

1. **Collect Data** → Gather thousands of examples (e.g., photos of cats and dogs)
2. **Train the Model** → Show the computer all the examples so it can find patterns
3. **Test the Model** → Show it new examples it has never seen before
4. **Improve** → Correct its mistakes so it gets better over time

---

#### 🧠 Deep Learning

**Deep Learning** is a more powerful type of machine learning. It uses structures called **neural networks** — which are inspired by the human brain.

Think of it like layers of thinking:

```
Input (Image) → Layer 1 (Detect edges) → Layer 2 (Detect shapes) → Layer 3 (Recognise face) → Output
```

Each layer learns something slightly more complex than the one before it. Deep learning is what powers face recognition on your phone and real-time translation apps.

---

#### 💬 Natural Language Processing (NLP)

**Natural Language Processing (NLP)** teaches computers to **understand human language** — reading, writing, and speaking.

> **Examples you already use:**
> - Asking **Siri, Alexa, or Google Assistant** a question → They use NLP to understand you
> - Your phone **autocompleting your text messages** → That's NLP predicting your next word
> - **Google Translate** converting Urdu to English → NLP at work

NLP is hard because human language is messy. "I saw the man with the telescope" — did you use the telescope, or did the man have it? Humans figure this out easily. Teaching a computer to do the same is a massive challenge.

---

#### 👁️ Computer Vision

**Computer Vision** gives computers the ability to **see and understand images and videos**.

> **Examples:**
> - Face unlock on your smartphone
> - Security cameras that detect suspicious behaviour automatically
> - Self-driving cars "seeing" traffic signs and pedestrians
> - Medical AI analysing X-ray images for tumours

---

#### 🦾 Robotics

**Robotics** is the science of designing, building, and programming **robots** — machines that can move and perform physical tasks.

Some robots follow fixed instructions (like a factory robot that paints cars). Advanced robots use AI to **sense** their environment, **make decisions**, and **adapt** to new situations.

> **Did You Know?** In Pakistan, robotics and AI-powered machines are being used in medical operations with greater precision than the human hand alone can achieve.

---

### 📊 Visual: Subfields of AI — The AI Family Tree

```
                    ARTIFICIAL INTELLIGENCE
                           │
        ┌──────────────────┼──────────────────┐
        │                  │                  │
  Machine Learning   Natural Language    Computer Vision
        │             Processing (NLP)        │
        │                                 (Seeing &
  Deep Learning                        Understanding
  (Neural Networks)                      Images)
        │
  Powers: Face ID,
  Speech Recognition,
  Medical Diagnosis
```

---

### ✋ Grab a Partner #2

> With a classmate, read these 5 scenarios. Decide which **subfield of AI** each one belongs to:
>
> 1. A phone app that translates your spoken Urdu sentence into written English
> 2. A robot arm that picks ripe tomatoes from a plant without damaging them
> 3. A system that watches CCTV footage and automatically flags people not wearing helmets
> 4. An app that reads thousands of customer reviews and says if they are "positive" or "negative"
> 5. A model that learns your music taste and creates a personalised playlist for you
>
> Write down your answers and check them at the end of the chapter!
> *(Answers: 1-NLP, 2-Robotics, 3-Computer Vision, 4-NLP, 5-Machine Learning)*

---

### ⚡ Quick Recap: Section 7.1

- **AI** = making computers think and learn like humans
- AI is used in healthcare, education, gaming, finance, agriculture, and much more
- AI has subfields: **ML, Deep Learning, NLP, Computer Vision, Robotics**
- Each subfield solves a different type of problem

> **One-sentence takeaway:** AI is not one technology — it is a whole family of technologies, each teaching computers a different kind of human skill.

---

## 7.2 AI Algorithms and Techniques

### 🎬 Story Mode: The Judge You Can't Question

Imagine you apply for a scholarship. A month later, you receive a letter: **"Application Rejected."** No reason. No explanation. You ask the admissions office why. They say: *"The computer decided."*

You feel frustrated. You cannot argue with a decision you do not understand.

Now imagine a different situation. The admissions officer says: *"Your application was rejected because your grade in Mathematics was below the minimum threshold of 75%, and the scholarship requires applicants from cities with less than 500,000 population."* You understand. You can improve. You can even appeal.

This difference — between a decision you can understand and one you cannot — is exactly what separates **Whitebox (Explainable)** AI from **Blackbox (Unexplainable)** AI.

---

### What Is an AI Algorithm?

An **algorithm** is a set of step-by-step instructions that a computer follows to solve a problem.

An **AI algorithm** is a special kind of algorithm that allows computers to **learn from data** and **make decisions** — often without being explicitly told what to do every step.

> **Analogy:** A regular recipe is an algorithm — follow steps A, B, C and you get a cake. An AI algorithm is different — you show the computer 10,000 photos of cakes and non-cakes, and it *figures out the recipe on its own.*

---

### 7.2.1 Types of AI Algorithms

All AI algorithms can be classified into two broad categories based on one important question:

> **Can a human understand WHY the AI made a particular decision?**

- If **YES** → it is a **Whitebox (Explainable)** algorithm
- If **NO** → it is a **Blackbox (Unexplainable)** algorithm

---

### 7.2.2 Explainable (Whitebox) Algorithms

**Whitebox algorithms** are transparent. You can look inside and see exactly why the AI made a decision. Every step of the decision process is visible and understandable.

> **Analogy:** Think of a whitebox algorithm like a glass box. You can see everything happening inside.

#### 🌳 Example: A Decision Tree

A **decision tree** is one of the most common whitebox algorithms. It makes decisions by asking a series of yes/no questions.

**Example: Should I carry an umbrella today?**

```
                    Is it raining?
                   /              \
                 YES               NO
                 /                  \
         Take umbrella        Is rain forecast?
                              /              \
                            YES               NO
                             /                 \
                     Take umbrella       Leave umbrella home
```

Every decision is traceable. You can follow the path and understand *exactly why* the AI said "take an umbrella." This is the power of a whitebox algorithm.

---

#### Other Examples of Whitebox Algorithms

- **Linear Regression** — predicts a number based on a straight-line formula (e.g., predicting house prices)
- **Rule-Based Systems** — a set of IF-THEN rules written by humans (e.g., "IF temperature > 39°C THEN flag as fever")
- **Decision Trees** — the example above

---

#### When Is Whitebox Important?

In high-stakes decisions — like **medical diagnosis**, **loan approvals**, or **court judgments** — it is critical that humans can *explain* and *audit* why the AI made a decision. In these cases, whitebox algorithms are preferred.

---

### 7.2.3 Unexplainable (Blackbox) Algorithms

**Blackbox algorithms** are the opposite. They are powerful — often *more accurate* than whitebox algorithms — but their decision-making process is hidden and difficult to understand, even for the scientists who built them.

> **Analogy:** Think of a blackbox algorithm like a sealed black box. You put in an input. An answer comes out. But what happened *inside* the box? Nobody is entirely sure.

---

#### 🧠 Example: Neural Networks

A **neural network** is a blackbox AI that is inspired by the human brain.

The human brain has billions of **neurons** (brain cells) connected to each other. When you learn something, connections between neurons grow stronger. Neural networks in AI work similarly.

**How a Neural Network is Structured:**

```
   INPUT LAYER          HIDDEN LAYERS           OUTPUT LAYER
   (Raw Data)          (Pattern Finder)          (Decision)

  ●  ●  ●  ●     →→→    ●  ●  ●           →→→      ●
                    →→→    ●  ●  ●           →→→
                    →→→    ●  ●  ●

  (e.g., pixels       (Detects edges,       (Says: "This is
   of an image)        shapes, features)      a cat.")
```

**Each layer learns something more complex:**

1. **Input Layer** → Receives raw data (e.g., pixel values of an image)
2. **Hidden Layer 1** → Detects basic patterns (edges, colours)
3. **Hidden Layer 2** → Recognises shapes (eyes, ears)
4. **Hidden Layer 3** → Identifies objects (a cat's face)
5. **Output Layer** → Gives the final answer ("It's a cat — 97% confident")

**Why is it a blackbox?** Because with millions of numbers inside those hidden layers, no human can trace exactly *which* pattern caused the AI to say "cat." The AI knows, in a mathematical sense — but it cannot explain it in human words.

---

#### Real-World Blackbox AI Examples

- **Deep Learning models** used in facial recognition
- **Language models** (like the ones powering AI assistants and chatbots)
- **AlphaGo** — Google DeepMind's AI that defeated the world champion of the game *Go* in 2016. This was considered nearly impossible because Go has more possible moves than there are atoms in the universe. Even AlphaGo's creators could not fully explain every move it made.

---

### 📊 Whitebox vs Blackbox: A Side-by-Side Comparison

| Feature | Whitebox (Explainable) | Blackbox (Unexplainable) |
|---|---|---|
| **Transparency** | High — you can see every step | Low — decisions are hidden |
| **Accuracy** | Moderate | Often very high |
| **Examples** | Decision Trees, Linear Regression | Neural Networks, Deep Learning |
| **Best used when** | Accountability matters (medical, legal) | Pure performance matters (image recognition) |
| **Can you explain it?** | Yes, easily | No, very difficult |

---

### ✋ Pause & Think #3

> Classify each of the following as **Whitebox** or **Blackbox** AI. Then explain your reasoning in one sentence.
>
> 1. A bank's AI that rejects a loan because: *"Income < PKR 30,000/month AND credit score < 600"*
> 2. A deep learning system that recognises your face to unlock your phone
> 3. A medical AI that says: *"Patient has fever. Rule: Fever + Cough = possible flu."*
> 4. A music streaming AI that recommends songs using a neural network with 50 hidden layers
>
> *(Answers: 1-Whitebox, 2-Blackbox, 3-Whitebox, 4-Blackbox)*

---

### 🤔 Ethical Corner: The Bias Problem

Here is something important to think about. AI algorithms — both whitebox and blackbox — learn from **data**. But what if the data is **biased**?

> **Example:** If an AI is trained only on photos of doctors who are male, it may learn to associate "doctor" with "male." Later, when it sees a female doctor, it might misclassify her as a nurse.

This is called **algorithmic bias**. It is not a reason to fear AI. It is an engineering problem — and the solution is to use **diverse, fair, and representative data**.

As a future tech creator, you will be responsible for building AI that is fair for everyone.

---

### ⚡ Quick Recap: Section 7.2

- An **AI algorithm** learns from data to make decisions
- **Whitebox algorithms** = transparent, explainable, traceable (e.g., Decision Trees)
- **Blackbox algorithms** = powerful but hard to explain (e.g., Neural Networks, Deep Learning)
- Both types have strengths and weaknesses — the right choice depends on the situation
- AI can be **biased** if trained on unfair data — this is a human responsibility to fix

> **One-sentence takeaway:** Whitebox AI shows its work like a student writing out every step; Blackbox AI gives the right answer but cannot show you how it got there.

---

## 7.3 Introduction to Internet of Things (IoT)

### 🎬 Story Mode: The Farm That Thinks for Itself

It is 3:00 AM. A farmer in rural Punjab is asleep. Back on his farm, a small sensor is buried in the soil. It notices that the soil moisture level has dropped below a critical level. It sends a signal — through a wireless network — to a central system. The system checks the weather forecast online: no rain predicted. So it sends a command to the water pump. The pump switches on automatically and waters the crops for exactly 22 minutes. Then it turns off.

The farmer wakes up at 7:00 AM and checks his phone. A notification reads: *"Crops watered at 3:12 AM. Water used: 450 litres. Soil moisture: Optimal."*

The farmer saved water. He saved time. He got a better night's sleep.

This is the **Internet of Things (IoT)** — and it is already changing farming, healthcare, homes, and cities across Pakistan and the world.

---

### 7.3.1 Understanding IoT: Definition and Significance

#### What Is IoT?

The **Internet of Things (IoT)** is a network of **physical objects** — everyday things — that are connected to the internet. These objects have sensors and software inside them. They collect data, share it, and sometimes act on it — **automatically**, without a human pressing a button.

The word **"Things"** here means any physical object: a water sensor, a smartwatch, a streetlight, a hospital bed, a car — anything.

> **In one sentence:** IoT means connecting everyday objects to the internet so they can collect, share, and act on data intelligently.

> **Historical Note:** The term "Internet of Things" was coined by **Kevin Ashton** in **1999** while working at Procter & Gamble. He used it to describe a system where physical objects were tagged and connected to the internet to track them automatically.

---

#### Why Does IoT Matter?

Before IoT, the physical world and the digital world were separate. If you wanted to know the temperature in a warehouse, a human had to go there and read a thermometer. If you wanted to turn off a light at home while you were away, you had to call someone.

IoT **bridges the gap** between the physical world and the digital world.

This means:
- **Better efficiency** — machines manage themselves, reducing waste
- **Better safety** — systems detect dangers and alert humans instantly
- **Better decisions** — constant data from the real world helps humans and AI make smarter choices
- **New services** — things that were impossible before become routine

> **Scale:** By the year 2020, there were already **over 20 billion IoT devices** in use worldwide. That number keeps growing every year.

---

### 7.3.2 Components of IoT Systems

An IoT system always has the same basic building blocks. Let's understand each one.

---

#### 📊 The IoT Data Flow: A Step-by-Step Picture

Here is how an IoT system works, from start to finish:

```
PHYSICAL WORLD                    DIGITAL WORLD
      │                                 │
   SENSORS          NETWORK         DATA ANALYSIS
  (Collect)    →→ (Transmit) →→   (Process & Decide)
      │                                 │
 ACTUATORS                         DEVICES / USER
  (Act / Do)   ←← (Command)  ←←  (App, Dashboard,
                                   Notification)
```

Now let's look at each component individually.

---

#### 1. 🌡️ Sensors — "The Eyes and Ears of IoT"

A **sensor** is a device that **detects and measures** something in the physical world and converts it into a digital signal.

**What can sensors measure?**

| Sensor Type | What It Measures | Example Use |
|---|---|---|
| Temperature sensor | How hot or cold it is | Smart thermostat, fever monitor |
| Humidity sensor | Moisture in the air | Smart farm, warehouse climate control |
| Motion sensor | Whether something is moving | Smart security camera, automatic door |
| Light sensor | How bright the light is | Automatic streetlights, phone screen brightness |
| Heart rate sensor | Your pulse | Smartwatch, hospital patient monitor |
| Soil moisture sensor | Water in soil | Smart irrigation system |

> **Key idea:** A sensor only *measures*. It does not act. It collects data and passes it on.

---

#### 2. ⚙️ Actuators — "The Hands of IoT"

An **actuator** is a device that **does something physical** based on a command it receives.

If a sensor is the "input" side of IoT, the actuator is the "output" side.

**Examples of actuators:**

- A **motor** that opens or closes a valve (e.g., turning on a water pump)
- A **relay switch** that turns a light on or off
- A **speaker** that plays an alarm sound
- A **door lock mechanism** that locks or unlocks a door

> **Key idea:** When the sensor says "soil moisture is too low," the actuator (water pump motor) acts on that information by switching on.

---

#### 3. 📱 Devices — "The Smart Objects"

**Devices** are the physical objects that are connected to the internet. They contain sensors and/or actuators and can communicate digitally.

**Examples:**

- Smartwatch (sensor: heart rate; device: the watch itself)
- Smart refrigerator (sensor: temperature inside; actuator: cooling motor)
- Smart traffic light (sensors detect car density; actuators change the signal timing)
- Connected car (thousands of sensors for speed, fuel, safety — all talking to a central system)

---

#### 4. 📡 Networks — "The Roads of IoT"

A **network** is the communication pathway that connects all IoT devices to each other and to the internet.

Without a network, devices are isolated. With a network, they become part of a connected system.

**Types of IoT Networks:**

| Type | Examples | Best For |
|---|---|---|
| **Wi-Fi** | Home routers | Smart homes, indoor devices |
| **Bluetooth** | Phone to smartwatch | Short-range, low power |
| **Cellular (4G/5G)** | SIM cards in devices | Remote locations, vehicles |
| **LoRaWAN** | Long-range, low-power signals | Smart farms, rural sensors |

---

#### 5. 📊 Data Analysis — "The Brain of IoT"

**Data analysis** is the process of **making sense of the data** that sensors collect.

Raw sensor data (e.g., "soil moisture = 18%") is just a number. Data analysis adds meaning: "18% is below the safe threshold of 30% — trigger irrigation."

Data analysis can happen in three places:

1. **On the device itself** (Edge Computing) — fast, no internet needed
2. **In the cloud** (Cloud Computing) — powerful, can process huge amounts of data
3. **On a central server** — a middle ground, used in hospitals and factories

---

### 📊 Full IoT System — Putting It All Together (Smart Farm Example)

```
┌───────────────────────────────────────────────────────────────┐
│                     SMART FARM IoT SYSTEM                     │
│                                                               │
│  1. SENSOR          2. NETWORK          3. DATA ANALYSIS      │
│  Soil moisture  →→  WiFi/LoRaWAN   →→  Cloud checks:         │
│  sensor reads       sends reading       "Moisture < 30%       │
│  "Moisture: 18%"    to cloud            → Water needed"       │
│                                                               │
│  6. FARMER          5. DEVICE           4. ACTUATOR           │
│  Gets phone     ←←  App shows:     ←←  Water pump            │
│  notification       "Crops watered"     switches ON           │
│  at 7 AM            successfully        for 22 minutes        │
└───────────────────────────────────────────────────────────────┘
```

---

### ✋ Grab a Partner #4

> Think about your own home. Identify **3 everyday objects** that could be made "smart" by adding sensors, a network connection, and an actuator.
>
> For each one, fill in this table:
>
> | Object | What sensor would it need? | What actuator would it control? | What problem would it solve? |
> |---|---|---|---|
> | Example: Water tap | Water flow sensor | Motor to close the tap | Stop water wastage when tap is left running |
> | 1. | | | |
> | 2. | | | |
> | 3. | | | |
>
> Share your ideas with the class. You might be designing the next great IoT product!

---

### 7.3.3 IoT Applications

Let's explore where IoT is already making a real difference.

---

#### 🏠 Smart Homes

A **smart home** is a house where everyday appliances are connected to the internet and can be controlled remotely or automatically.

**Examples:**

- **Smart thermostat** → learns your temperature preferences and adjusts automatically, saving energy
- **Smart lighting** → turns off lights in empty rooms, saving electricity
- **Smart security camera** → detects motion, sends alerts to your phone, records footage
- **Smart door lock** → you can unlock your front door from anywhere using your phone
- **Smart refrigerator** → tracks food items and tells you when something is about to expire

> **Did You Know?** Smart home devices can cut your electricity bills significantly by automatically turning off appliances when they are not needed.

---

#### 🏥 Healthcare IoT

IoT is saving lives in hospitals and homes.

**How it works:**

1. A patient in a hospital wears a wearable sensor on their wrist
2. The sensor continuously monitors heart rate, blood oxygen, temperature, and blood pressure
3. Data is sent wirelessly to a central nursing station
4. If any reading goes outside the safe range, an **alarm triggers automatically**
5. A nurse is alerted *before* the patient's condition becomes dangerous

**Other healthcare IoT examples:**

- **Smart pill bottles** that remind patients to take their medication and alert family if a dose is missed
- **Remote patient monitoring** for patients recovering at home after surgery
- **Smart hospital beds** that detect if a patient has fallen or moved out of position

> **Safety Tip:** Always use devices from trusted manufacturers and protect your health data with strong passwords.

---

#### 🚗 Transportation IoT

IoT is making roads smarter and safer.

**Examples:**

- **Smart traffic lights** → sensors count cars at intersections and adjust signal timing to reduce traffic jams
- **Vehicle-to-Vehicle (V2V) communication** → cars talk to each other wirelessly to warn about sudden braking or accidents ahead
- **Predictive vehicle maintenance** → sensors inside cars detect when a part is about to fail and alert the driver *before* a breakdown occurs
- **Real-time bus tracking** → passengers can see exactly where their bus is using an app

---

#### ✋ Activity: Design Your Smart School

> Think about your school. Imagine you are the principal and you have an unlimited IoT budget.
>
> Answer these questions:
>
> 1. What sensor would you put in the library to track available seats?
> 2. How would you use IoT to save electricity in classrooms?
> 3. How would you use IoT to make the school bus safer?
> 4. What data would your smart school collect every day?
>
> Draw a simple diagram of your **IoT-enabled school** showing:
> - At least 4 sensors
> - The network connecting them
> - Where the data goes
> - At least 2 actuators
>
> Present your design to the class!

---

### 7.3.4 Security and Privacy Considerations in IoT Deployments

### 🎬 Story Mode: The Unlocked Front Door

In 2016, hackers took control of **millions of IoT devices** — security cameras, smart routers, and even baby monitors — all because the device owners had never changed the factory default password. The hackers used these devices together like an army to attack major websites. This became known as the **Mirai Botnet Attack** — one of the largest cyberattacks in history.

Nobody had been careful. Nobody had changed their passwords. And everyday home devices became weapons.

This is the serious side of IoT. **More connected devices = more entry points for hackers.**

---

#### Why Is IoT Security So Important?

Every IoT device that connects to the internet is a potential **entry point** for a cyberattack. Unlike computers and phones (which get regular security updates and have strong antivirus software), many IoT devices are:

- Small and low-power, with limited security features
- Running old software that is never updated
- Shipped from factories with default passwords that users never change
- Connected to networks 24 hours a day, 7 days a week

---

#### Common IoT Security Threats

| Threat | What It Means | Real Example |
|---|---|---|
| **Unauthorised Access** | A hacker logs into your device | Hacker watching through your home CCTV camera |
| **Data Interception** | Hacker reads data being transmitted | Stealing health data from a patient monitor |
| **Device Hijacking** | Hacker takes control of your device | Using your smart speaker to spy on you |
| **Botnet Attack** | Hacker uses your device to attack others | Mirai Botnet — millions of hacked IoT devices |

---

#### ✅ How to Protect Your IoT Devices — Security Best Practices

---

**1. 🔑 Use Strong, Unique Passwords**

Every IoT device needs a strong password. A strong password:

- Has at least 12 characters
- Includes uppercase letters, lowercase letters, numbers, and symbols
- Is different for every device
- Is NEVER the factory default (e.g., never keep "admin/admin")

> **Bad password:** 1234, admin, password
> **Good password:** Pk$m@rt2024#ioT

---

**2. 🔄 Keep Software Updated Regularly**

Manufacturers release **firmware updates** to fix security vulnerabilities. If you do not update your device, old vulnerabilities remain open for hackers to exploit.

> **Rule:** When your IoT device says "Update Available" — update it immediately.

---

**3. 🔒 Use Encryption**

**Encryption** converts data into a coded format so that even if a hacker intercepts it, they cannot read it.

> **Analogy:** Imagine writing a letter and putting it in a locked box. Even if someone steals the box, they cannot read the letter without the key.

Make sure your IoT devices transmit data over **encrypted connections** (look for HTTPS, TLS, or WPA2/WPA3 for Wi-Fi).

---

**4. 📶 Use a Secure, Separate Network**

Connect your IoT devices to a **separate Wi-Fi network** (called a "guest network" or "IoT network"), away from your main computer and phone. This way, if a hacker compromises an IoT device, they cannot access your personal files.

---

**5. 🏭 Buy from Reputable Manufacturers**

Choose IoT devices made by known, trusted companies that take security seriously. Cheap, unknown-brand devices often skip security features to reduce costs.

---

### 🔒 Privacy: Who Is Watching Your Data?

IoT devices collect enormous amounts of data about you:

- Your **home temperature preferences** (smart thermostat)
- Your **location at all times** (smartwatch, connected car)
- Your **health metrics** (fitness band, hospital monitor)
- Your **daily routines** (when you wake up, when you leave home)

**Who can see this data?**

- The device manufacturer
- The cloud service provider
- Potentially, government agencies (in some countries)
- Hackers (if the system is not secured)

**Your rights as a user:**

- Read the **privacy policy** before using any IoT device
- Turn off data collection features you do not need
- Use devices from companies with clear, transparent data policies

---

### ✋ Pause & Think #5

> Read the following scenario and answer the questions:
>
> *Ayesha's school installs smart cameras in every classroom. The cameras use AI to detect if students are paying attention, looking at their phones, or falling asleep. The data is sent to a server that the school administration can access.*
>
> 1. What are **two benefits** of this system?
> 2. What are **two serious privacy concerns** this raises?
> 3. Do you think this is fair? Would you want cameras like this in your classroom?
> 4. What rules would you put in place if you were the school principal?
>
> There is no single right answer. This is a real ethical debate happening in schools around the world right now.

---

### ⚡ Quick Recap: Section 7.3

- **IoT** connects everyday physical objects to the internet so they can collect and share data
- An IoT system has 5 key components: **Sensors, Actuators, Devices, Networks, Data Analysis**
- IoT applications include **smart homes, healthcare, transportation, agriculture**
- IoT faces serious **security threats** — unauthorised access, data interception, device hijacking
- Protect IoT devices with **strong passwords, regular updates, encryption, and secure networks**

> **One-sentence takeaway:** IoT makes everyday objects smart by connecting them to the internet — but every connected device is also a responsibility to keep secure.

---

## Chapter Summary

Let's bring everything together.

```
┌─────────────────────────────────────────────────────────────────┐
│              UNIT 7: EMERGING TECHNOLOGIES — BIG PICTURE        │
│                                                                 │
│  ARTIFICIAL INTELLIGENCE (AI)                                   │
│  ├── Makes computers THINK and LEARN like humans                │
│  ├── Applied in: Healthcare, Education, Finance, Gaming, etc.   │
│  ├── Subfields: ML, Deep Learning, NLP, Computer Vision,        │
│  │              Robotics                                        │
│  └── Algorithms:                                                │
│       ├── Whitebox (Explainable) → Decision Trees               │
│       └── Blackbox (Unexplainable) → Neural Networks            │
│                                                                 │
│  INTERNET OF THINGS (IoT)                                       │
│  ├── Connects physical objects to the internet                  │
│  ├── Components: Sensors → Network → Data Analysis              │
│  │               → Actuators → Devices                          │
│  ├── Applications: Smart Homes, Healthcare, Transportation,     │
│  │                 Agriculture                                  │
│  └── Security: Strong passwords, Updates, Encryption            │
│                                                                 │
│  SHARED CHALLENGES:                                             │
│  ├── Data Privacy → Who owns your data?                         │
│  ├── Algorithmic Bias → Is the AI fair to everyone?             │
│  └── Security Risks → More connections = more vulnerabilities   │
└─────────────────────────────────────────────────────────────────┘
```

---

## Exercises

### Multiple Choice Questions

Circle the best answer:

**1.** Which of the following is NOT a subfield of AI?

- a) Machine Learning
- b) Natural Language Processing
- c) Computer Vision
- **d) DBMS**

**2.** Which of these is a security concern in IoT deployments?

- a) Device vulnerability
- b) Data privacy
- c) Lack of standardisation
- **d) All of the above**

**3.** Which of the following is an application of AI in healthcare?

- a) Personalised drug development
- b) Automated diagnosis
- c) Remote patient monitoring
- **d) All of the above**

**4.** What is the primary purpose of using AI techniques in machine learning models?

- a) To improve accuracy
- b) To enhance interpretability
- c) To reduce computational complexity
- **d) All of the above**

**5.** What is the key difference between explainable (whitebox) and unexplainable (blackbox) AI models?

- a) The complexity of the model
- **b) The ability to understand the decision-making process**
- c) The performance of the model
- d) The training data used

**6.** Which of the following is an application of IoT in the transportation domain?

- a) Smart traffic management
- b) Vehicle-to-Vehicle (V2V) communication
- c) Predictive maintenance of vehicles
- **d) All of the above**

---

### Short Answer Questions

Answer each question in 3–5 sentences:

**1.** Define Artificial Intelligence (AI).

**2.** Provide two examples of AI applications in healthcare. For each example, explain the benefit it brings to patients.

**3.** Explain the role of AI techniques in advancing machine learning models. How does "learning from data" make a model better over time?

**4.** Define the Internet of Things (IoT). Use a real-world example from Pakistan to explain your definition.

**5.** Describe the significance of IoT in connecting devices and systems. Why does this matter for everyday life?

**6.** Describe three specific applications of IoT in the transportation domain. For each one, explain what problem it solves.

---

### Critical Thinking Questions

These questions have no single right answer. Think carefully and write your opinion with reasons:

**7.** A hospital wants to use a blackbox AI to diagnose cancer from X-rays. The AI is 96% accurate — more accurate than most human doctors. But no one can explain *how* it makes its decisions. Should the hospital use it? What safeguards would you put in place?

**8.** Your city wants to install IoT sensors on every street corner to monitor air quality, noise levels, and foot traffic. This data would help city planners design better roads and parks. But the sensors could also track where you go every day. Is this a good idea? What privacy rules should govern it?

---

### Activity: IoT System Design Challenge

Design a complete IoT system for **one of the following scenarios**. Draw a diagram and label every component:

- **Scenario A:** A smart classroom that automatically adjusts lighting, temperature, and records attendance
- **Scenario B:** A smart water tank for a home that monitors water level and automatically refills from a pump
- **Scenario C:** A smart school bus that tracks location, monitors student boarding/departure, and alerts parents

Your diagram must include:

1. At least **3 sensors** (label what each one measures)
2. The **network** type you would use and why
3. Where **data analysis** happens (device, cloud, or server)
4. At least **2 actuators** (label what each one does)
5. How the **user** (student, parent, teacher, etc.) receives information or control

---

## Glossary of Key Terms

| Term | Simple Definition |
|---|---|
| **Artificial Intelligence (AI)** | Technology that allows computers to think, learn, and make decisions like humans |
| **Machine Learning (ML)** | A type of AI where computers learn from examples and data, without being programmed for every step |
| **Deep Learning** | A powerful type of ML that uses neural networks — layers of calculations inspired by the human brain |
| **Neural Network** | An AI system modelled after the human brain, with layers that each learn something more complex |
| **Natural Language Processing (NLP)** | AI technology that allows computers to understand and generate human language |
| **Computer Vision** | AI technology that enables computers to see, interpret, and understand images and videos |
| **Robotics** | The science of designing, building, and programming robots that can perform physical tasks |
| **Whitebox Algorithm** | An AI algorithm whose decision-making process is transparent and understandable |
| **Blackbox Algorithm** | An AI algorithm whose decision-making process is hidden and difficult to explain |
| **Decision Tree** | A whitebox AI model that makes decisions through a series of yes/no questions |
| **Algorithmic Bias** | When an AI makes unfair decisions because it was trained on incomplete or biased data |
| **Internet of Things (IoT)** | A network of physical objects connected to the internet, capable of collecting and sharing data |
| **Sensor** | A device that detects and measures physical properties (temperature, light, motion) |
| **Actuator** | A device that performs a physical action (opening a valve, switching on a motor) in response to a command |
| **Encryption** | Converting data into a coded format so that only authorised parties can read it |
| **Firmware** | Built-in software on a device that controls its hardware functions |
| **Edge Computing** | Processing IoT data directly on the device, without sending it to the cloud |
| **Botnet** | A network of hacked devices controlled by an attacker to carry out cyberattacks |

---

## Partner Activity Answers (Check Your Work!)

**Grab a Partner #2 Answers:**

1. A phone app that translates spoken Urdu into written English → **NLP**
2. A robot arm that picks ripe tomatoes → **Robotics**
3. A system that watches CCTV and flags people without helmets → **Computer Vision**
4. An app that reads reviews and classifies them as positive/negative → **NLP**
5. A model that learns your music taste and creates playlists → **Machine Learning**

**Pause & Think #3 Answers:**

1. "Income < PKR 30,000/month AND credit score < 600" → **Whitebox** (clear rules)
2. Face recognition using deep learning → **Blackbox** (neural network)
3. "Fever + Cough = possible flu" → **Whitebox** (rule-based)
4. Music recommendation using 50-layer neural network → **Blackbox** (deep learning)

---

*End of Unit 7: Emerging Technologies in Computer Science*

---

> **A Final Word from Your Teacher:**
> You just completed one of the most important chapters in modern computer science. AI and IoT are not distant future concepts — they are happening right now, in Pakistan and across the world. The engineers, designers, policymakers, and thinkers who will shape these technologies are sitting in classrooms exactly like yours. Maybe one of them is you.
>
> Keep asking questions. Keep thinking critically. And never stop being curious.
