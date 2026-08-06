# Chapter 2: System Recovery and Advanced Maintenance
### *An Interactive Learning Journey for 10th Class Computer Science*

---

> **A Note Before We Begin:**
> Every expert computer technician you have ever seen — the person who fixes your school's computers, the IT guy at the office, the engineer at the repair shop — they all started exactly where you are right now. They did not know any of this. They learned it one step at a time.
>
> In this chapter, you will make mistakes. You might get confused. That is 100% normal. Confusion means your brain is working hard. Keep going. By the end of this chapter, you will understand how computers fix themselves, protect themselves, and recover from problems — and so will you.

---

## 2.1 Introduction to Post-Troubleshooting

---

### 🎬 The Hook — Story Mode

**A Historical Story: The World's First Computer "Bug"**

The year was **1947**. A brilliant scientist named **Grace Hopper** was working on one of the earliest computers in the world, called the **Mark II**. It was a huge machine — as big as an entire room — filled with switches, wires, and metal parts.

One day, the machine stopped working. Grace and her team searched and searched for the problem. After hours of looking, they finally found it: a **real moth** — a tiny flying insect — was trapped inside one of the machine's switches. The moth was causing the circuit to fail.

Grace carefully removed the moth with a pair of tweezers. She taped it into the team's logbook and wrote next to it: *"First actual case of bug being found."*

That is where the word **"bug"** in computing comes from. And that is where the word **"debugging"** — fixing a computer problem — comes from too.

But here is the important part: **after removing the moth, the team did not just walk away.** They checked all the other switches. They cleaned the machine. They made notes about what happened. They wanted to make sure the same problem never happened again.

That careful work *after* fixing the problem? That is exactly what this chapter is about.

---

**A Relatable Scenario: The Bicycle Chain**

Imagine your bicycle chain slips off. You put it back on — problem solved, right?

But a smart cyclist does not stop there. They ask:

- *Why did the chain slip?*
- *Is the chain too loose? Is it worn out?*
- *When was the last time I oiled it?*

If they do not think about these questions, the chain will slip again next week, and then again the week after. Real fixing means fixing the **root cause** and then **taking care of things regularly** so the problem does not return.

Computers work the exact same way.

---

### 📘 The Core Blueprint — 5W1H

**WHAT is Post-Troubleshooting Maintenance?**

**Troubleshooting** means finding and fixing a computer problem. For example: restarting the system, checking cables, or reinstalling a program.

**Post-troubleshooting maintenance** means the *additional care* you give the computer *after* the problem is already fixed.

Think of it this way:
- Troubleshooting = treating the illness.
- Post-troubleshooting = the recovery plan after leaving the hospital.

This maintenance includes: cleaning up the system, checking for future risks, updating software, and making sure the same problem does not return.

---

**WHY do we need it?**

Without regular maintenance, a computer becomes like a room that is never cleaned. Problems silently build up:

| Problem | What Happens Without Maintenance |
|---|---|
| **Slow Performance** | Temporary files pile up, unused programs run in the background, RAM gets wasted. The computer becomes slow and unresponsive. |
| **System Failures** | Important updates are missed. The computer may freeze, crash, or refuse to start. |
| **Security Risks** | Old, unpatched software has security holes. Viruses and harmful programs can enter easily. |
| **Data Loss** | Without backups, a single crash can destroy months of school work or family photos. |
| **Hardware Damage** | Dust builds up inside the computer. Heat cannot escape. Components overheat and get damaged permanently. |

---

**WHO uses it?**

Post-troubleshooting maintenance is done by:

- **Everyday users** (like you!) who want their home computer to stay fast and safe.
- **Students** who store school work and want to keep it safe.
- **School IT staff** who manage many computers in a computer lab.
- **Office workers** who rely on computers for their daily tasks.
- **Professional computer technicians** who are hired to repair and maintain systems.

You do not have to be an expert. You just have to be consistent.

---

**WHERE does it happen?**

Maintenance happens in several places:

- **Inside the computer** — cleaning dust from fans and vents (physical maintenance).
- **In the operating system** — using Windows tools like Task Manager, Disk Cleanup, and Windows Defender.
- **In software settings** — checking for updates, managing startup programs, and reviewing error logs.

---

**WHEN do we do it?**

You should perform maintenance:

- **After fixing a problem** — always. This prevents the same issue from coming back.
- **On a regular schedule** — for example, once a week or once a month (we will build a maintenance calendar in Section 2.6).
- **When the computer feels slow** — before the problem gets serious.
- **Before major events** — before exams, presentations, or important work, check that everything is running well.

---

**HOW does it work? — The System Health Monitoring Concept**

Modern operating systems like **Microsoft Windows** have built-in tools that help you watch the health of your computer. This is called **System Health Monitoring**.

These tools allow you to:

- See how much memory (RAM) and processing power (CPU) are being used right now.
- Watch which programs are running quietly in the background.
- Read warning and error messages the computer has recorded.
- Find which programs are slowing your computer down.

By checking these things regularly, you can catch small problems before they become big ones.

---

### 🛠️ The Practical Walkthrough — Your First Health Check

Here is a simple first step to check the health of your computer right now:

**Step 1:** Look at your computer. Is it running slowly? Are any programs frozen?

**Step 2:** Think about when you last restarted it. Restarting clears temporary memory and is the simplest form of maintenance.

**Step 3:** Think about when you last deleted old files or emptied the Recycle Bin.

**Step 4:** Think about when the computer last received a software update.

If you answered "I don't know" to most of these, that is okay! By the end of this chapter, you will have a clear plan. Let's start building it together.

---

### 💡 Pause & Think — Stop Point #1

> **Challenge:** You fixed your computer — it was running slowly, and you deleted some old files. It feels better now.
>
> But three weeks later, it is slow again.
>
> **Question:** What did you probably forget to do? Write down at least **3 things** you should have done *after* fixing the problem the first time that might have prevented the slowness from coming back.
>
> Discuss your answers with a partner. There are no wrong answers here — just thinking.

---

## 2.2 Using Built-in Diagnostic Tools

---

### 🎬 The Hook — Story Mode

**A Historical Story: The Cockpit Dashboard**

When the Wright Brothers flew the first airplane in 1903, the pilot had almost no information. He could feel the wind. He could see the ground. That was it. If something went wrong, he found out the hard way — by crashing.

Today, a modern airplane cockpit is filled with hundreds of instruments: screens, gauges, warning lights, and sensors. The pilot does not need to "feel" if something is wrong. The instruments tell them *exactly* what is happening — which engine is working, how much fuel is left, what the temperature is.

This completely changed aviation safety. Problems are caught early, before they become disasters.

Your computer has its own "cockpit" — a set of built-in tools that show you exactly what is happening inside. You just need to know how to read them.

---

**A Relatable Scenario: Your School Report Card**

Imagine you are a teacher, and you want to know if a student is struggling. You do not just guess. You look at their **report card** — marks, attendance, behavior notes.

A computer's diagnostic tools are its "report card." They show you which programs are using too much memory, which ones are misbehaving, and what errors have occurred.

---

### 📘 The Core Blueprint — 5W1H

**WHAT are Built-in Diagnostic Tools?**

These are special programs that come **already installed** inside Windows. You do not need to download anything. They let you see what is happening inside your computer in real time.

There are three main tools you need to know:

1. **Task Manager** — the quick overview tool.
2. **Resource Monitor** — the detailed investigation tool.
3. **Event Viewer** — the error history tool.

Think of them as three different types of doctors:
- Task Manager is like a general doctor — gives you a quick checkup.
- Resource Monitor is like a specialist — goes deep into one specific area.
- Event Viewer is like a historian — shows you everything that happened in the past.

---

**WHY do we need them?**

Without these tools, you would have to guess why your computer is slow or why it crashed. These tools remove the guessing. They give you **exact facts**:

- Which program is using 90% of your RAM?
- Which background process is secretly downloading data?
- What error message appeared at 3:00 AM when the computer crashed?

With this information, you can fix problems correctly — not randomly.

---

**WHO uses them?**

- Students and home users — to end frozen programs and check system health.
- IT technicians — to diagnose slow or crashing systems professionally.
- Network administrators — to monitor which programs are using internet bandwidth.

---

**WHERE are they found?**

All three tools are built into **Microsoft Windows**. They do not require installation. You access them through keyboard shortcuts or the Windows search bar.

---

**WHEN do we use them?**

| Tool | Use It When... |
|---|---|
| **Task Manager** | Your computer is slow or a program has stopped responding ("Not Responding"). |
| **Resource Monitor** | You need more detail — e.g., the computer is hot, using a lot of memory, but you do not know why. |
| **Event Viewer** | The computer crashed or showed an error, and you want to find out exactly what happened and when. |

---

**HOW does each tool work?**

Let us go through each one.

---

### 🛠️ Tool 1: Task Manager — The Quick Overview

**How to Open Task Manager:**

There are two easy ways:

- **Method A:** Press **Ctrl + Shift + Esc** on your keyboard simultaneously. Task Manager opens immediately.
- **Method B:** Right-click on the **Taskbar** (the bar at the bottom of your screen). Select **"Task Manager"** from the menu.

---

**What you will see inside Task Manager:**

Task Manager has several tabs. The two most important for you are:

**The Processes Tab:**

- Shows a **list of every program currently running** on your computer.
- For each program, it shows how much **CPU** (processing power) and **Memory** (RAM) it is using.
- Programs using very high percentages are the ones slowing your computer down.

**The Performance Tab:**

- Shows **live graphs** — moving lines that go up and down in real time.
- You can see CPU usage, RAM usage, Disk usage, and Network usage — all happening right now.
- If the CPU graph is near 100% all the time, your computer is working too hard.

---

**How to End a Frozen Program (Step by Step):**

This is the most common thing you will use Task Manager for.

- **Step 1:** Open Task Manager using **Ctrl + Shift + Esc**.
- **Step 2:** Click on the **"Processes"** tab at the top.
- **Step 3:** Look through the list. Find the program that is frozen or not responding. It may say **"(Not Responding)"** next to its name.
- **Step 4:** Click on that program's name once to select it (it will be highlighted in blue).
- **Step 5:** Click the **"End Task"** button at the bottom right of the window.
- **Step 6:** The program will close. The computer may feel faster immediately.

> ⚠️ **Important:** Only end a task if you are sure it is a program you recognize. Do NOT end tasks with names like "System," "Windows Explorer," or "Antimalware Service." These are important for Windows to work.

---

### 🛠️ Tool 2: Resource Monitor — The Detailed Investigation

**How to Open Resource Monitor:**

- **Method A:** Open Task Manager → Click the **"Performance"** tab → At the very bottom, click **"Open Resource Monitor."**
- **Method B:** Press **Windows key + R**. A small box appears. Type **`resmon`** and press **Enter**.

---

**What you will see inside Resource Monitor:**

Resource Monitor has four tabs. Each one shows a different part of your computer's activity:

| Tab | What It Shows |
|---|---|
| **CPU Tab** | Which processes and services are using the processor. |
| **Memory Tab** | How much RAM is being used, how much is free, and how much is reserved. |
| **Disk Tab** | Which programs are reading from or writing to the hard drive right now. |
| **Network Tab** | Which applications are sending or receiving data over the internet. |

**When is this useful?**

If your computer is extremely slow and Task Manager shows memory usage is high, open Resource Monitor. Go to the Memory tab. Find the program using the most memory. That is your culprit.

---

### 🛠️ Tool 3: Event Viewer — The History Book

**How to Open Event Viewer:**

- Press **Windows key + R**.
- Type **`eventvwr`** in the box.
- Press **Enter**.

---

**What you will see inside Event Viewer:**

Event Viewer is like a diary that Windows keeps automatically. Every time something important happens — an error, a warning, a program crash — Windows writes it down here with the exact **date and time**.

The entries are organized into types:

- **Error** — Something went wrong. Red circle with an X.
- **Warning** — A potential problem was detected. Yellow triangle.
- **Information** — A normal event was recorded. Blue circle with an "i."

**When is this useful?**

Your computer crashed last night while you were sleeping. In the morning, you want to know why. Open Event Viewer, look at the errors from that time, and you will see exactly what happened.

---

### 💡 Grab a Partner — Stop Point #2

> **Challenge:** Open Task Manager right now on your computer.
>
> 1. Go to the **Processes** tab. Write down the **top 3 programs using the most CPU** and the **top 3 programs using the most Memory**.
> 2. Now switch to the **Performance** tab. Look at the CPU graph. Is it mostly flat (low usage) or going up and down a lot (high usage)?
> 3. Compare your answers with a partner. Are the same programs appearing on both computers? Why or why not?
>
> **Discussion question:** If one program is using 80% of the CPU, what do you think would happen if you ended that task?

---

## 2.3 System Recovery Options

---

### 🎬 The Hook — Story Mode

**A Historical Story: The NASA Apollo 13 Mission**

In April 1970, three astronauts were flying to the Moon on Apollo 13. Suddenly, an oxygen tank inside the spacecraft exploded.

The mission to land on the Moon was immediately cancelled. But the real question now was: *how do we get these three astronauts home alive?*

The team at NASA in Houston did not panic. They had **backup plans**. They had **recovery procedures**. They switched the astronauts from the main spacecraft into the small Lunar Module — a backup vehicle that was designed for landing on the Moon, not for traveling home. They used it as a "lifeboat."

They also had to restart the main spacecraft — which had been turned off to save power — using a very careful, step-by-step checklist. One wrong step could have been fatal.

The three astronauts returned home safely.

The lesson: **Good systems always have recovery options.** When the main plan fails, you fall back to the backup plan. Windows is built exactly this way.

---

**A Relatable Scenario: The School Notebook**

Imagine you accidentally spilled water on your notebook and some pages got damaged. But you had been making **photocopies** of important pages every week. You go to your folder, pull out the photocopy from last week, and you are safe.

System recovery options are Windows's way of making photocopies of your system before things go wrong.

---

### 📘 The Core Blueprint — 5W1H

**WHAT are System Recovery Options?**

These are special tools built into Windows that help you **restore the computer to a working state** when something has gone badly wrong — beyond what basic troubleshooting can fix.

There are three main recovery options:

1. **Safe Mode** — Start Windows in a minimal, stripped-down version to fix problems.
2. **System Restore** — Take the computer back to how it was on a specific earlier date.
3. **Bootable Recovery Media** — Start the computer from a USB drive when Windows cannot even load.

---

**WHY do we need them?**

Some problems are too serious for a simple restart. For example:

- You installed a driver and now Windows crashes every time it starts.
- A virus has infected the system and it keeps freezing.
- Windows will not load at all — you just see a black screen.

In these cases, recovery options are your safety net.

---

**WHO uses them?**

Any computer user may need these one day. IT technicians use them daily. Students who install software from untrusted sources may need them. Parents who accidentally install a bad program may need them.

---

**WHERE are they found?**

- Safe Mode: accessed during the startup process or through Windows Settings.
- System Restore: found in Control Panel > System and Security > System > System Protection.
- Bootable Media: created in advance on a USB drive.

---

**WHEN do we use each one?**

| Recovery Option | Use It When... |
|---|---|
| **Safe Mode** | The system keeps crashing or freezing. You want to uninstall a bad program or scan for a virus. |
| **System Restore** | After installing a program or driver, Windows started behaving badly. You want to go back to before you made that change. |
| **Bootable Recovery Media** | Windows will not even start. Safe Mode is not accessible. You need to repair or reinstall Windows. |

---

### 🛠️ Practical Walkthrough 1: Using Safe Mode

**WHAT is Safe Mode?**

Safe Mode starts Windows using only the **most essential programs and drivers**. All unnecessary background software is disabled. This makes it much easier to find and fix a problem caused by a bad app or setting.

Think of Safe Mode like this: imagine your house has hundreds of lights on. Something is wrong, but you cannot tell which light is causing the electrical problem. So you turn **almost all the lights off**, leave only the important ones on, and now you can find the problem much more easily. Safe Mode turns off most of Windows's extra programs so you can see what is causing the trouble.

---

**HOW to Enter Safe Mode (Modern Windows 10 / 11):**

- **Step 1:** Click the **Start** button (Windows logo in the bottom left corner).
- **Step 2:** Click the **Settings** gear icon.
- **Step 3:** Go to **Update & Security**.
- **Step 4:** On the left side, click **Recovery**.
- **Step 5:** Under "Advanced Startup," click **"Restart Now."**
- **Step 6:** Your computer will restart and show a blue menu. Choose **Troubleshoot**.
- **Step 7:** Click **Advanced Options**.
- **Step 8:** Click **Startup Settings**.
- **Step 9:** Click **Restart**.
- **Step 10:** Your computer restarts again and shows a numbered list. Press the **F4** key to enter Safe Mode.

**Alternative for older computers:**

Restart the computer. Before the Windows logo appears, press **F8** repeatedly. Select **Safe Mode** from the menu and press **Enter**.

---

## Method 1: The Shift + Restart Shortcut (Fastest)

If you can see a power button anywhere on your screen (either on the desktop Start menu or on the login screen before you even sign in), you can skip the Settings menu entirely.

1. **Find a Power Button:** On desktop or login screen.
Open your Start menu OR look at the bottom-right corner of your sign-in screen to find the **Power** icon.


2. **Shift + Click Restart:** Crucial timing dependency.
Press and **hold down the Shift key** on your keyboard, and while holding it, click **Restart**.


3. **Navigate the Blue Menu:** Familiar recovery screen.
Keep holding Shift until the blue "Choose an option" screen appears. From here, follow the same path as your original list: **Troubleshoot** > **Advanced options** > **Startup Settings** > **Restart**.


---

## Method 2: System Configuration Tool (`msconfig`)

This method is useful if you want Windows to automatically boot into Safe Mode every single time you restart, without pressing any special keys.

> ⚠️ **Important Note:** Once you turn this on, your PC will *keep* booting into Safe Mode until you go back into this tool and turn it off.

1. **Open Run:** Shortcut.
Press the **Windows Key + R** on your keyboard to open the Run dialog box.


2. **Launch System Configuration:** Command.
Type `msconfig` into the box and press **Enter**.


3. **Enable Safe Boot:** Configuration.
Click on the **Boot** tab at the top of the window. Under "Boot options" at the bottom, check the box next to **Safe boot**. Leave it on "Minimal" for standard Safe Mode.


4. **Apply and Restart:** Execution.
Click **Apply**, then click **OK**. A prompt will pop up asking if you want to restart now. Click **Restart**.


---

## Method 3: The Hard Hard Reboots (Emergency Failsafe)

If Windows is completely frozen, crashing on startup, or showing a blank screen, you can force the system into the recovery menu using the physical power button on your computer.

1. **Force Shutdown:** Interrupted boot 1.
Press and hold your PC's physical power button for about 10 seconds to force it completely off.


2. **Interrupt the Boot:** Interrupted boot 2.
Turn the PC back on. The moment you see the manufacturer logo (like HP, Dell, Lenovo) or the spinning Windows loading circles, **immediately press and hold the physical power button again** to force it off.


3. **Repeat Once More:** Interrupted boot 3.
Repeat Step 2 one more time. (You are intentionally interrupting the boot process twice in a row).


4. **Access Recovery Mode:** Automatic trigger.
Turn the PC on a third time and let it boot completely. Windows will detect the failed startups and automatically load the **Preparing Automatic Repair** screen, followed by the blue recovery menu. Select **Advanced options** > **Troubleshoot** to reach your Startup Settings.

---

**Safe Mode with Networking:**

This is a special version of Safe Mode that also allows internet access. You use it when:

- You need to download a driver or update to fix the problem.
- You want to use an online antivirus scanner.

To enter Safe Mode with Networking, follow all the same steps above but press **F5** instead of F4 in Step 10.

---

> ⚠️ **Safety Rules for Using Safe Mode:**
> - Do not delete files unless your teacher or a trusted expert tells you to.
> - Do not change settings you do not understand.
> - When finished, restart the computer normally — Safe Mode is not meant for regular use.

---

### 🛠️ Practical Walkthrough 2: System Restore

**WHAT is System Restore?**

System Restore takes your computer's settings back to how they were on a specific earlier date. It does **not** delete your personal files (photos, documents, etc.). It only reverses changes to system settings, installed programs, and drivers.

**What is a Restore Point?**

A restore point is like a **photograph of your system** taken at a specific moment. It captures what programs are installed, what settings are in place, and how drivers are configured.

Windows creates restore points automatically:

- Before a system update is installed.
- Before a new driver is installed.
- On a regular schedule.

You can also create one manually whenever you want.

---

**HOW to Create a Restore Point Manually (Step by Step):**

Do this BEFORE making any major changes to your computer (like installing a new program or driver).

- **Step 1:** Click the **Start** button and search for **"Control Panel."** Open it.
- **Step 2:** Click on **"System and Security."**
- **Step 3:** Click on **"System."**
- **Step 4:** On the left side, click **"System Protection."** A new window opens.
- **Step 5:** Make sure the drive (usually C:) shows **"Protection: On."** If not, click "Configure" and turn it on.
- **Step 6:** Click the **"Create"** button.
- **Step 7:** Type a name that will help you remember when and why you created this restore point. For example: *"Before installing printer driver – 4 June 2026."*
- **Step 8:** Click **"Create."** Wait a few seconds.
- **Step 9:** A message will say "The restore point was created successfully." Click **Close.**

---

*Some other methods*

## Method 1: The Windows Search Shortcut (Fastest GUI Route)

You can skip the Control Panel entirely by using Windows Search to jump directly to the **System Properties** window where restore points are managed.

1. **Open Windows Search:** Shortcut.
Press the **Windows Key** on your keyboard or click the Start menu.


2. **Search for the Tool:** Keyword.
Type **"Restore Point"** or **"Create a restore point"** into the search bar.


3. **Jump Directly to the Settings:** Execution.
Press **Enter** or click the top match. This bypasses the Control Panel entirely and opens the exact **System Protection** window you need. From here, follow your original steps to click **Create** and name it.


---

## Method 2: Using Command Prompt (Admin)

If you prefer using the command line or need to create a restore point when the standard desktop interface isn't responding well, you can do it with a single command line.

1. **Open Command Prompt as Admin:** Elevated access.
Press the **Windows Key**, type `cmd`, right-click on **Command Prompt**, and select **Run as administrator**.


2. **Run the WMI Command:** Command string.
Copy and paste the following command, then press **Enter**:

```cmd
wmic.exe /Namespace:\\root\default Path SystemRestore Call CreateRestorePoint "Manual Restore Point", 100, 7

```


3. **Check the Output:** Verification.
The terminal will execute the command. If successful, you will see a return value of `0`, meaning your restore point has been created in the background.


---

## Method 3: Using PowerShell (Best for Automation)

PowerShell offers a clean, modern cmdlet to handle restore points. This is especially useful if you want to understand how Windows handles automation scripts.

1. **Open PowerShell as Admin:** Elevated access.
Right-click the **Start button** (or press `Win + X`) and select **Terminal (Admin)** or **Windows PowerShell (Admin)**.


2. **Execute the Cmdlet:** Command string.
Type the following command (you can change the text inside the quotes to whatever description you prefer) and press **Enter**:

```powershell
Checkpoint-Computer -Description "BeforeMajorChange" -RestorePointType "MODIFY_SETTINGS"

```


3. **Wait for the Progress Bar:** Progress indicator.
A progress bar will appear at the top of the PowerShell window. Once it reaches 100% and returns to the command prompt, your restore point is safe and active.


---

**HOW to Use a Restore Point to Fix a Problem (Step by Step):**

Use this when your computer started behaving badly after a recent change.

- **Step 1:** Open **Control Panel.**
- **Step 2:** Click **"Recovery."**
- **Step 3:** Click **"Open System Restore."** A wizard (step-by-step guide) opens.
- **Step 4:** Click **"Next."**
- **Step 5:** A list of restore points appears. Select the most recent one that was created **before** the problem started.
- **Step 6:** Click **"Next"**, then click **"Finish."**
- **Step 7:** A warning will appear: "Once started, System Restore cannot be interrupted." Click **"Yes."**
- **Step 8:** Your computer will restart automatically. The restoration process will happen. When it finishes, Windows will load normally and show a confirmation message.

---

### 🛠️ Practical Walkthrough 3: Bootable Recovery Media

**WHAT is Bootable Recovery Media?**

This is a **USB flash drive or DVD** that contains special system files. It can start your computer even if the hard drive or Windows is completely broken.

**Think of it like an emergency key.** If the main door to your house is broken, you use a spare key you kept somewhere safe. Bootable media is that spare key for your computer.

---

**WHAT can you do with it?**

When you boot from a recovery USB, you can:

- **Startup Repair** — Fix problems that stop Windows from loading.
- **System Restore** — Use a restore point even when Windows will not start.
- **Command Prompt** — Advanced troubleshooting (for experts).
- **System Reset or Reinstallation** — Reinstall Windows completely as a last resort.

---

**UNDERSTANDING GPT vs MBR — The Partition Styles:**

Before creating a bootable USB, you must know one important concept.

Every storage drive (hard drive or SSD) needs to be organized using a **partition style** — a system that tells the computer how data is arranged on the drive.

There are two types:

| Feature | MBR (Master Boot Record) | GPT (GUID Partition Table) |
|---|---|---|
| **Age** | Older (from the 1980s) | Modern standard |
| **Maximum Disk Size** | Up to 2 TB only | More than 2 TB |
| **Maximum Partitions** | Only 4 primary partitions | Over 100 partitions |
| **Used With** | Older BIOS systems | Modern UEFI systems |

**Why does this matter for your bootable USB?**

If your computer uses **UEFI**, you must create the USB with **GPT** format.
If your computer uses **older BIOS**, you must create the USB with **MBR** format.
If they do not match, the computer will not be able to boot from the USB.

---

**HOW to Check Your Computer's Partition Style:**

- **Step 1:** Press **Windows key + X** on your keyboard. A menu appears.
- **Step 2:** Click **"Disk Management."**
- **Step 3:** Look at the list of disks. Find **"Disk 0"** — that is usually where Windows is installed.
- **Step 4:** Right-click on the **"Disk 0"** label on the left side of the screen.
- **Step 5:** Select **"Properties."**
- **Step 6:** Click the **"Volumes"** tab.
- **Step 7:** Look at the **"Partition Style"** field. It will say either **GUID Partition Table (GPT)** or **Master Boot Record (MBR).** Now you know which format to use.

---

**HOW to Create a Bootable USB Using Rufus (Step by Step):**

*Rufus is a free, safe tool for creating bootable USB drives. It is only for Windows.*

- **Step 1:** Get a USB drive with at least **16 GB** of storage space. Warning: all files on the USB will be deleted, so back them up first.
- **Step 2:** Download the Windows ISO file (system image) from the official Microsoft website.
- **Step 3:** Download **Rufus** from its official website: **https://rufus.ie/en/**
- **Step 4:** Plug the USB drive into your computer.
- **Step 5:** Open Rufus.
- **Step 6:** Under **"Device,"** select your USB drive from the dropdown list.
- **Step 7:** Under **"Boot selection,"** click **"SELECT"** and choose the ISO file you downloaded.
- **Step 8:** Under **"Partition scheme,"** select **GPT** (for modern UEFI computers) or **MBR** (for older BIOS computers), based on what you found in your Disk Management check.
- **Step 9:** Click **"START."**
- **Step 10:** A warning will appear saying all data on the USB will be destroyed. Click **"OK"** to confirm.
- **Step 11:** Wait for Rufus to finish. When it says **"READY"** at the bottom, your bootable USB is complete.

Here are the alternative methods for both checking your partition style and creating a bootable USB drive, optimized for speed, terminal usage, and cross-platform flexibility.

---

## Part 1: Alternate Methods to Check Your Partition Style

The Disk Management GUI is reliable, but using the command line is significantly faster, especially if you are working with multiple disks or remote systems.

### Method 1: Using PowerShell (Fastest & Clearest)

PowerShell provides a clean, readable table that lists all connected drives and their partition styles instantly.

1. **Open PowerShell as Admin:** Elevated access.
Right-click the **Start button** (or press `Win + X`) and select **Terminal (Admin)** or **Windows PowerShell (Admin)**.


2. **Run the Get-Disk Cmdlet:** Command string.
Type the following command and press **Enter**:

```powershell
Get-Disk

```


3. **Read the Style Column:** Verification.
Look at the output table under the **Partition Style** column. It will clearly list **GPT** or **MBR** for every disk connected to your system.


---

### Method 2: Using Command Prompt (`diskpart`)

This traditional method works on any modern or legacy version of Windows, including recovery environments where PowerShell might not be available.

1. **Open Command Prompt as Admin:** Elevated access.
Press the **Windows Key**, type `cmd`, right-click on **Command Prompt**, and select **Run as administrator**.


2. **Launch Diskpart:** Utility initialization.
Type `diskpart` and press **Enter**. The prompt will change to `DISKPART>`.


3. **List Connected Disks:** Inventory query.
Type `list disk` and press **Enter**.


4. **Check the GPT Column:** Analysis.
Look at the far-right column labeled **Gpt**. If there is an **asterisk (*)** next to a disk, it is using **GPT**. If the column is blank for that disk, it is using **MBR**.


---

## Part 2: Alternate Methods to Create a Bootable USB

While Rufus is the go-to tool on Windows, these alternatives offer automation or cross-platform compatibility (working on Linux and macOS as well).

### Method 1: The Official Windows Media Creation Tool (Easiest)

If you are installing Windows on a modern GPT/UEFI system, Microsoft’s official tool handles downloading the ISO and burning it to the USB all in one automated process, skipping Rufus entirely.

1. **Connect Storage:** Preparation.
Plug in your blank 16GB+ USB drive.


2. **Download the Tool:** Acquisition.
Go to the official Microsoft software download page and download the **Media Creation Tool** for your specific Windows version.


3. **Launch and Accept Terms:** Initialization.
Run the downloaded tool and accept the license terms.


4. **Choose Media Creation Type:** Selection.
When asked what you want to do, select **"Create installation media (USB flash drive, DVD, or ISO file) for another PC"** and click Next.


5. **Target the USB Drive:** Execution.
Choose **USB flash drive**, select your drive letter from the list, and click Next. The tool will automatically download the correct, updated Windows installer file and configure the USB partition scheme.


---

### Method 2: Using Ventoy (Best Multi-Boot / Drag-and-Drop Method)

Ventoy is a game-changing alternative. Instead of formatting your USB every time you want a new installer, you install Ventoy to the USB *once*, and then you simply **copy and paste raw ISO files** onto the drive like a regular flash drive. It even allows you to store multiple operating systems (e.g., Windows 10, Windows 11, and Linux) on a single USB.

1. **Download Ventoy:** Acquisition.
Download and extract the Ventoy tool from its official site or GitHub repository.


2. **Install Ventoy to the USB:** Setup.
Open `Ventoy2Disk.exe`, select your USB flash drive, and click **Install**. This creates a special, secure boot partition on the drive.


3. **Drag and Drop ISO Files:** Deployment.
Open your regular Windows File Explorer, click on your newly formatted Ventoy USB drive, and simply drag and drop your downloaded Windows ISO file directly into the drive space.


> 💡 **Why Ventoy shines:** When you boot from this USB, a clean text menu appears letting you choose which ISO you want to run. If a new version of Windows drops, you just delete the old ISO file and paste the new one in—no reinstalling or re-flashing required.

---

### 💡 Pause & Think — Stop Point #3

> **Challenge:** You installed a new graphics driver three days ago. Since then, your screen flickers every few minutes. You want to fix it.
>
> **Question:** Which recovery option would you use — Safe Mode, System Restore, or Bootable Media? Write out the **exact reason** for your choice.
>
> Bonus: At what point in the process would it have been smart to create a restore point? Before or after installing the driver? Why?

---

## 2.4 BIOS/UEFI and Boot Process Awareness

---

### 🎬 The Hook — Story Mode

**A Historical Story: The Birth of BIOS**

In the early 1980s, IBM was building the very first **IBM Personal Computer** (IBM PC 5150). The engineers faced a critical challenge: how does a computer "wake up"?

When you flip a light switch, electricity immediately flows. But a computer is far more complicated. It has a CPU, RAM, a hard drive, a keyboard, a display — many different parts. When power turns on, *something* must tell the computer how to check all these parts and get everything ready before Windows can even start loading.

The engineers created a small chip on the motherboard — the main circuit board of the computer — with a tiny program burned into it. This program would run **immediately** when power turned on, before anything else. It would check the hardware, prepare everything, and then hand control over to the operating system.

They called it the **BIOS** — Basic Input/Output System.

It was a revolutionary idea in 1981. Today, almost every computer in the world still uses a descendant of that idea — either a BIOS or its modern replacement, the UEFI.

---

**A Relatable Scenario: The School Morning Routine**

Before your first class begins, the school does a set of morning checks: the security guard unlocks the gates, the teachers arrive, the classrooms are unlocked, the attendance system is turned on.

Nobody can start learning until all these preparations are complete.

The BIOS/UEFI is the computer's "morning routine." Before Windows can load, it checks that all the hardware is ready to go.

---

### 📘 The Core Blueprint — 5W1H

**WHAT is BIOS/UEFI?**

**Firmware** is a special type of software that is stored **permanently on a chip on the computer's motherboard.** It is not stored on the hard drive. It does not get deleted when the computer is turned off or when Windows is reinstalled.

There are two types of firmware:

- **BIOS (Basic Input/Output System):** The older type. It shows a simple, text-only menu with a black or blue background. You can only control it with the keyboard. It was standard in computers from the 1980s through the early 2000s.

- **UEFI (Unified Extensible Firmware Interface):** The modern replacement for BIOS. It shows a graphical menu — often with colors, mouse support, and even images. It is faster, supports larger hard drives, and is more secure. Most computers made after 2012 use UEFI.

---

**WHY do we need BIOS/UEFI?**

BIOS/UEFI serves three critical functions:

1. **Hardware Check:** It checks that all the essential hardware — RAM, keyboard, hard drive — is connected and working correctly.
2. **Boot Device Selection:** It finds which device has the operating system (e.g., the hard drive or a USB) and tells the computer to start loading from it.
3. **System Configuration:** It stores basic settings like the date, time, and boot order.

Without BIOS/UEFI, the computer would turn on and have absolutely no idea what to do.

---

**WHO uses it?**

Most users never need to touch BIOS/UEFI. But it becomes important when:

- A technician is setting up a new computer.
- You need to boot from a USB drive to reinstall Windows.
- You want to change the order in which the computer looks for a bootable device.
- Something is wrong at the hardware level and you need to diagnose it.

---

**WHERE is it found?**

BIOS/UEFI is stored on a small chip on the **motherboard** — the main circuit board inside the computer. You access its settings screen by pressing a specific key during startup, before Windows loads.

---

**WHEN do we access it?**

- When you need to **change the boot order** (e.g., to boot from a USB drive first).
- When you need to **reset BIOS settings to default** after something went wrong.
- When a **POST error** occurs and you need to investigate.

---

### 🛠️ The POST Test — Your Computer's Pre-Flight Check

**WHAT is POST?**

**POST** stands for **Power-On Self-Test.**

Every single time your computer turns on, before Windows even begins to load, the BIOS/UEFI automatically runs the POST. This is a quick internal test that checks the most important hardware components.

**HOW does POST work?**

- **Step 1:** Power is turned on.
- **Step 2:** BIOS/UEFI chip wakes up immediately.
- **Step 3:** POST begins — it checks:
  - Is the CPU (processor) working?
  - Is the RAM (memory) present and functional?
  - Is the keyboard connected?
  - Is the hard drive present?
- **Step 4:** If **everything passes**, POST finishes silently. You see the computer manufacturer's logo, and then Windows begins to load.
- **Step 5:** If **something fails**, the computer cannot continue. It alerts you in one of two ways:
  - **Beep codes** — a series of beeps (e.g., one long beep followed by two short beeps means a specific problem). Different BIOS manufacturers have different beep patterns.
  - **Error message on screen** — a text message describing what failed.

**Example:** If the RAM is not properly connected, the computer will beep continuously and refuse to start. Reconnecting the RAM and restarting allows POST to pass successfully.

---

### 🛠️ Practical Walkthrough: Accessing BIOS/UEFI

**HOW to Open BIOS/UEFI Settings:**

The key to press depends on your computer's brand. Common keys are listed below:

| Computer Brand | BIOS/UEFI Key |
|---|---|
| Dell | F2 or F12 |
| HP | Esc or F10 |
| Lenovo | F1 or F2 |
| ASUS | Del or F2 |
| Acer | Del or F2 |
| MSI | Del |
| Surface (Microsoft) | Volume Down button |

You must press the key **very quickly** — the window is only about 1-2 seconds during startup.

**Step-by-Step:**

- **Step 1:** Completely shut down your computer (not sleep — fully shut down).
- **Step 2:** Press the **Power button** to turn it on.
- **Step 3:** Immediately and repeatedly press the BIOS key for your computer brand (e.g., **Del** or **F2**).
- **Step 4:** The BIOS/UEFI screen appears. You are now inside the firmware settings.
- **Step 5:** Use your keyboard (BIOS) or mouse (UEFI) to navigate. Do not change anything unless you know exactly what it does.
- **Step 6:** To exit without saving changes, press **Esc** or select **"Exit Without Saving."**

---

**HOW to Change the Boot Order:**

You need to change the boot order when you want the computer to start from a USB drive (e.g., to use a bootable recovery USB) instead of the hard drive.

- **Step 1:** Enter BIOS/UEFI settings using the steps above.
- **Step 2:** Look for a tab or section called **"Boot"** or **"Boot Options."**
- **Step 3:** You will see a list of devices — for example: Hard Drive, USB Drive, CD/DVD Drive, Network.
- **Step 4:** Move your USB drive to the **top of the list** (the computer tries devices from top to bottom).
- **Step 5:** Press **F10** to save and exit (or find the "Save and Exit" option in the menu).
- **Step 6:** Your computer restarts and now boots from the USB drive first.

---

**HOW to Reset BIOS to Default Settings:**

If wrong settings have been saved and the computer is behaving strangely:

- Enter BIOS/UEFI.
- Look for an option called **"Load Setup Defaults"**, **"Reset to Default"**, or **"Restore Defaults."**
- Select it and confirm.
- Save and exit.

This resets all settings to factory defaults — the same settings the computer had when it left the factory.

---

### 💡 Pause & Think — Stop Point #4

> **Challenge:** Your computer is beeping three times every time you turn it on, and it does not load Windows. The screen stays black.
>
> **Questions:**
> 1. What part of the boot process is this happening in — before or after POST?
> 2. What do the beeps mean?
> 3. What is your first step to try to fix this problem?
>
> Hint: Think about what POST is checking and what a "beep code" means.

---

## 2.5 Data Recovery Techniques

---

### 🎬 The Hook — Story Mode

**A Historical Story: The Voyager 1 Spacecraft**

NASA launched the Voyager 1 spacecraft in 1977. It is now the farthest human-made object in space — billions of kilometers from Earth.

In 2023, scientists on Earth noticed that Voyager 1 was sending back garbled, meaningless data. The spacecraft was so far away that a radio signal took 22.5 hours just to travel from Earth to Voyager and back. 

What had happened? A chip in one of Voyager's three onboard computers had developed a **memory corruption problem** — like a kind of data damage in space. The engineers could not physically go to the spacecraft. They had to figure out how to recover the data and fix the computer from 24 billion kilometers away.

After months of careful work, they figured out the problem, rerouted the data around the damaged memory chip, and Voyager began sending correct data again.

If NASA can recover data from a spacecraft 24 billion kilometers away, you can absolutely recover a deleted file from your computer.

---

**A Relatable Scenario: Dropping Your Notebook in a Puddle**

You accidentally drop your school notebook in a muddy puddle. Some pages are fine. Some are damaged. A few are completely destroyed.

Data recovery is like carefully drying out the notebook, seeing which pages can still be read, and photographing the ones that survived. Not everything may be saved — but you might recover more than you expect.

---

### 📘 The Core Blueprint — 5W1H

**WHAT is Data Recovery?**

Data recovery is the process of **finding and restoring files** that have been accidentally deleted, lost due to a system crash, or damaged by a hardware or software problem.

---

**WHY do we need it?**

Because accidents happen. A student accidentally deletes their final project file. A crash happens and the file is gone. A USB drive is removed improperly and files become corrupted.

Data recovery gives us a second chance to get those files back.

---

**WHO uses it?**

Everyone. Students, office workers, photographers, small business owners — anyone who has ever accidentally deleted something important.

---

**WHERE do we find recovery tools?**

- **Built-in tools** are already inside Windows — Recycle Bin, File History, Previous Versions.
- **Third-party tools** are programs you download and install — like **Tenorshare 4DDiG.**

---

**WHEN do we use data recovery?**

- When you accidentally delete a file.
- When a file becomes corrupted (opens but shows garbage characters).
- After a system crash causes files to disappear.
- When a USB drive or memory card fails.

---

**HOW does data recovery actually work? — The Science Behind It**

This is fascinating. When you delete a file in Windows, the computer does **not** immediately destroy the data.

Instead, it does something clever: it simply **removes the "label"** — the file name and location record — and marks that storage space as "available for reuse."

The actual data is still there on the drive. It is just like removing the label from a box in a warehouse. The box (and its contents) is still physically there — it is just not listed in the catalog anymore. Anyone who looks carefully can still find it.

Data recovery software works by **scanning the drive and looking for these "unlabeled boxes."** It finds data that is still physically present but no longer indexed, and it rebuilds the connection.

**Important:** This only works if the computer has not yet **written new data over that space.** Once new data fills that area, the old file is truly gone. This is why speed matters in data recovery — the sooner you try to recover a file, the better your chances.

---

### 🛠️ Practical Walkthrough 1: Built-in Recovery Tools

**Method A — The Recycle Bin (Easiest Method)**

When you delete a file in Windows, it goes to the **Recycle Bin** first. It stays there until you manually empty the Recycle Bin.

- **Step 1:** Find the **Recycle Bin** icon on your desktop (it looks like a trash can).
- **Step 2:** Double-click it to open it.
- **Step 3:** Look through the files listed inside.
- **Step 4:** Find the file you want to recover. Right-click on it.
- **Step 5:** Select **"Restore."**
- **Step 6:** The file will instantly return to its original location on your computer.

> 📝 This method only works if you have NOT already emptied the Recycle Bin.

---

**Method B — File History (For Scheduled Backups)**

File History is a feature in Windows that automatically saves copies of your files at regular intervals to an external drive. If it was turned on before the problem occurred, you can recover older versions of files.

**How to Turn On File History (do this NOW before problems happen):**

- **Step 1:** Go to **Settings** (press Windows key + I).
- **Step 2:** Click **"Update & Security."**
- **Step 3:** Click **"Backup"** on the left side.
- **Step 4:** Connect an external USB hard drive or flash drive to your computer.
- **Step 5:** Under "Back up using File History," click **"Add a drive."**
- **Step 6:** Select your external drive from the list.
- **Step 7:** Turn on the toggle that says **"Automatically back up my files."**

Windows will now automatically back up your Documents, Pictures, Desktop, and other important folders to that drive at regular intervals.

**How to Recover a File Using File History:**

- **Step 1:** Go to **Settings > Update & Security > Backup.**
- **Step 2:** Click **"More options."**
- **Step 3:** Scroll down and click **"Restore files from a current backup."**
- **Step 4:** Browse through the backup history to find the version of the file you need.
- **Step 5:** Select the file and click the **green Restore button.**

---

**Method C — Previous Versions**

This feature lets you recover an earlier saved version of a specific file or folder.

- **Step 1:** Navigate to the file or folder that you want to recover.
- **Step 2:** Right-click on it.
- **Step 3:** Select **"Properties."**
- **Step 4:** Click the **"Previous Versions"** tab.
- **Step 5:** If previous versions are available, they will be listed with their dates.
- **Step 6:** Select the version you want to restore.
- **Step 7:** Click **"Restore."**

> 📝 Previous Versions only works if System Protection or File History was previously enabled.

---

### 🛠️ Practical Walkthrough 2: Using Tenorshare 4DDiG (Third-Party Tool)

When the Recycle Bin has been emptied and no backup exists, you need a third-party recovery tool. **Tenorshare 4DDiG** is a safe, beginner-friendly option.

**HOW to Use Tenorshare (Step by Step):**

- **Step 1:** Download and install Tenorshare from its official website. **Important:** Install it on a **different drive** than the one where you lost the file. For example, if your file was lost from the **C: drive**, install Tenorshare on the **D: drive** or on an external USB. Installing on the same drive could overwrite the lost data.

- **Step 2:** Open Tenorshare.

- **Step 3:** The program will ask you to **select a location.** Choose the drive or folder where the lost file was saved (e.g., Desktop, C: drive, USB drive).

- **Step 4:** Choose the **type of file** you are looking for — Pictures, Documents, Videos, Audio, etc. Selecting a specific type makes the scan faster.

- **Step 5:** Click the **"Scan"** button. The program will begin scanning the drive for deleted or lost files. This may take a few minutes depending on the drive size.

- **Step 6:** When the scan finishes, a list of recoverable files will appear. Browse through them to find your file.

- **Step 7:** Select the file(s) you want to recover.

- **Step 8:** Click **"Recover."** A dialog box will ask where to save the recovered files. Choose a **different drive** or a different folder — do not save to the same location where the file was lost.

---

**Limitations of Data Recovery — The Honest Truth:**

Data recovery is powerful, but it is not magic. You should know its limits:

- If the file was deleted **a long time ago** and the computer has been used heavily since then, the data may have been overwritten by new files. Recovery may fail.
- If the **hard drive is physically damaged** (dropped, water damaged), software recovery tools may not work. Physical repair by a specialist is required.
- If the Recycle Bin was emptied **and no backup was ever made**, and the space has been overwritten, the file is **permanently gone.**

---

> 💡 **Two Golden Rules of Data Recovery:**
>
> **Rule 1:** Check the Recycle Bin FIRST. It is the easiest and fastest method. Do not skip it.
>
> **Rule 2:** Never install recovery software on the same drive where your lost file was stored. This can overwrite the deleted data and make recovery impossible.

---

### 💡 Pause & Think — Stop Point #5

> **Challenge:** Your younger sister was working on a school project. She saved the file on the Desktop. Then she accidentally pressed **Delete** and then emptied the Recycle Bin. She is crying.
>
> **Question:** Walk through the recovery process, step by step, from easiest to hardest option:
> 1. What is the first thing you check? (Already done — Recycle Bin is empty)
> 2. What is your second option? (Think: did anyone set up File History on this computer?)
> 3. What is your third option if no backup exists?
> 4. What is the most important rule to remember when you try to recover the file?

---

## 2.6 Best Practices for Preventive Maintenance

---

### 🎬 The Hook — Story Mode

**A Historical Story: The Titanic and Predictable Disasters**

On April 14, 1912, the Titanic — the largest and most advanced ship of its time — struck an iceberg and sank. More than 1,500 people lost their lives.

Historians have studied this disaster for over a century. And one of the most important findings is this: **the disaster was preventable.** The ship was traveling too fast in dangerous waters. The crew had received iceberg warnings and did not slow down. There were not enough lifeboats. Maintenance of the watertight compartments was inadequate.

The Titanic disaster was not just bad luck. It was the result of **a failure to take preventive action** when the warning signs were there.

Computer failures are rarely sudden surprises. They almost always give warnings first — a computer getting slower, a hard drive making strange noises, a virus warning popping up. **Preventive maintenance** means listening to those warnings and acting before the disaster happens.

---

**A Relatable Scenario: Your Health**

A doctor does not just treat you when you are sick. They also tell you: wash your hands regularly, eat vegetables, exercise, get enough sleep. These are **preventive measures** — they stop you from getting sick in the first place.

Computer maintenance is the same idea. You do not just fix problems when they appear. You do small, regular tasks that stop problems from appearing at all.

---

### 📘 The Core Blueprint — 5W1H

**WHAT is Preventive Maintenance?**

Preventive maintenance means performing **regular, scheduled tasks** to keep a computer running well — before any problem actually occurs.

These tasks include: cleaning up disk space, installing software updates, scanning for viruses, and keeping a maintenance schedule.

---

**WHY do we need it?**

Because prevention is always easier than cure.

- A disk cleanup done monthly takes 5 minutes. A system rebuild after a failure caused by full storage takes hours or days.
- A security update installed today takes 5 minutes. Recovering from a virus attack caused by not installing that update can take days and may result in permanent data loss.

---

**WHO does it?**

All computer users should practice basic preventive maintenance. In schools and offices, IT staff perform these tasks on all computers on a regular schedule.

---

**WHERE do the maintenance tasks happen?**

Inside the Windows operating system using built-in tools.

---

**WHEN should maintenance be done?**

On a regular schedule. We will build a specific maintenance calendar at the end of this section.

---

### 🛠️ Maintenance Task 1: Disk Cleanup

**WHAT is Disk Cleanup?**

Over time, your computer silently collects unnecessary files:

- **Temporary internet files** — pieces of websites saved on your drive to load pages faster.
- **System cache files** — temporary data created by Windows during normal operation.
- **Windows Update files** — old update packages that are no longer needed.
- **Recycle Bin contents** — files you deleted but that are still taking up space.

These files do nothing useful. They just take up valuable storage space and can slow the computer down.

**Disk Cleanup** is a built-in Windows tool that finds and safely removes all these unnecessary files.

---

**HOW to Run Disk Cleanup (Step by Step):**

- **Step 1:** Click the **Windows search bar** (bottom left of the screen, next to the Start button).
- **Step 2:** Type **"Disk Cleanup"** and press **Enter.** The tool opens.
- **Step 3:** A small window appears asking you to choose which drive to clean. Select **"C:"** (this is usually where Windows and your main files are stored). Click **"OK."**
- **Step 4:** Wait a few seconds while the tool calculates how much space can be freed.
- **Step 5:** A list of file categories appears with checkboxes. Each category shows how much space will be freed. Common ones include:
  - Temporary Internet Files
  - Recycle Bin
  - Temporary Files
  - System error memory dump files
- **Step 6:** Check the boxes next to the categories you want to delete.
- **Step 7:** Click **"OK."** A confirmation message appears.
- **Step 8:** Click **"Delete Files."** The cleanup runs and the selected files are deleted.

> ✅ **Recommended:** Run Disk Cleanup once a month for best performance.

---

### 🛠️ Maintenance Task 2: Software Updates (Patch Management)

**WHAT are software updates?**

Software developers regularly release **updates** — also called **patches** — for their programs. These updates:

- Fix security holes that hackers could exploit.
- Fix bugs (errors) in the software.
- Add new features and improvements.
- Improve how the program works with other software.

There are two types of updates:

1. **Operating System Updates** — Updates for Windows itself (or macOS, Linux, etc.).
2. **Application Updates** — Updates for individual programs (like your web browser, media player, PDF reader, etc.).

---

**HOW to Check for and Install Windows Updates (Step by Step):**

- **Step 1:** Press **Windows key + I** to open **Settings.**
- **Step 2:** Click **"Update & Security."**
- **Step 3:** Make sure you are on the **"Windows Update"** section (it is usually selected by default).
- **Step 4:** Click **"Check for updates."**
- **Step 5:** Windows will check Microsoft's servers for any new updates.
- **Step 6:** If updates are available, they will be listed. Click **"Download and Install."**
- **Step 7:** Some updates require a restart. When prompted, save your work and restart the computer.

> ✅ **Recommended:** Check for updates once a week. Turn on automatic updates if you tend to forget.

---

### 🛠️ Maintenance Task 3: Virus Scanning with Windows Defender

**WHAT is Windows Defender?**

**Windows Defender** (also called **Windows Security**) is the built-in antivirus and security program in Windows. It protects your computer from:

- **Viruses** — programs that damage files or spread to other computers.
- **Malware** — harmful software that spies on you, steals data, or takes control of your computer.
- **Spyware** — programs that secretly monitor what you type and do.
- **Ransomware** — programs that lock your files and demand payment.

---

**HOW to Run a Virus Scan (Step by Step):**

- **Step 1:** Click the **Windows search bar** and type **"Windows Security."** Press **Enter.**
- **Step 2:** Click **"Virus & threat protection."**
- **Step 3:** You will see two scan options:
  - **Quick Scan** — checks the most common locations where viruses hide. Faster (usually a few minutes).
  - **Full Scan** — checks every single file on your computer. Thorough but slow (can take 1-2 hours).
- **Step 4:** Click **"Quick Scan"** for a routine check. Click **"Scan options"** → **"Full Scan"** for a deep check.
- **Step 5:** Click **"Scan now."** Windows Defender will scan and report any threats found.
- **Step 6:** If threats are found, follow the on-screen instructions to remove or quarantine them.

---

**Real-Time Protection — Your 24-Hour Guard:**

Windows Defender also has a feature called **Real-Time Protection.** This means it is constantly watching in the background — even when you are not running a scan. If it detects a suspicious file being downloaded or opened, it immediately blocks it and alerts you.

To make sure Real-Time Protection is active:

- Open **Windows Security.**
- Click **"Virus & threat protection."**
- Click **"Virus & threat protection settings."**
- Make sure **"Real-time protection"** is toggled **ON.**

> ✅ **Recommended:** Run a Quick Scan once a week. Run a Full Scan once a month.

---

### 🛠️ Maintenance Task 4: Your Personal Maintenance Calendar

A maintenance calendar is a simple schedule that tells you **when to do which maintenance task.** It prevents you from forgetting important tasks.

Here is a suggested maintenance calendar you can follow:

| Frequency | Task |
|---|---|
| **Every week** | Check for Windows and app updates. Run a Quick Scan in Windows Defender. |
| **Every month** | Run Disk Cleanup. Run a Full Scan in Windows Defender. Check available storage space. |
| **Every 3 months** | Create a manual System Restore point. Check all cables and physical connections. |
| **Every 6 months** | Clean dust from the computer vents (using compressed air). Review and delete old files you no longer need. |
| **Every year** | Review all installed programs — uninstall anything you no longer use. |

You can write this in a paper planner, set reminders on your phone, or use the calendar app on your computer. The tool does not matter. The habit does.

---

### 💡 Grab a Partner — Stop Point #6

> **Challenge:** You and your partner are the new IT managers of your school's computer lab. The lab has 30 computers. Students use them daily.
>
> **Task:** Create a maintenance plan for the lab. Answer these questions together:
>
> 1. Which tasks need to be done **every week?**
> 2. Which tasks need to be done **every month?**
> 3. Who is responsible for doing each task — the students, the teacher, or the IT manager?
> 4. What would happen to the computers after **6 months of no maintenance?** List at least 3 specific problems you would expect.

---

## 2.7 System Documentation and Logs

---

### 🎬 The Hook — Story Mode

**A Historical Story: A Doctor's Medical Records**

Imagine you go to a new doctor because your regular doctor moved to another city. The new doctor sits down with you and says: "I need to know your medical history." 

If your previous doctor kept good records — every visit, every medicine, every test result — the new doctor can pick up exactly where the last one left off. They know what treatments worked and which ones did not. They can make better decisions faster.

But if your previous doctor kept no records, the new doctor starts from zero. They might repeat tests you already had. They might not know you are allergic to a certain medicine. They might miss something important.

**Medical records save lives.** Computer maintenance logs serve the same purpose.

---

**A Relatable Scenario: The Recipe Book**

Your grandmother makes an amazing biryani. The secret is in the exact amounts and method. If she keeps a recipe book, anyone can make the same biryani — even after she is gone. If she remembers it only in her head, the recipe is lost the moment she cannot cook anymore.

A system log is your computer's recipe book. It records exactly what was done, when, and why — so that anyone who comes later (including future you) can understand what happened and continue from there.

---

### 📘 The Core Blueprint — 5W1H

**WHAT is System Documentation and Logs?**

**System documentation** means keeping organized written records of everything you do to a computer — installations, repairs, updates, errors, and maintenance tasks.

**System logs** (generated automatically by the computer) are records that Windows writes on its own — recording errors, warnings, and system events with exact timestamps.

Together, these records create a complete history of a computer system.

---

**WHY do we need it?**

Imagine a computer in your school has been fixed three times this year for the same problem. If nobody wrote down what was done each time, the technician fixes the same thing over and over without understanding the root cause.

With proper documentation:

- You can see patterns — "This computer keeps failing every 3 months. It must be a hardware issue."
- A new technician can understand the computer's history without starting from scratch.
- You can prove that maintenance was done (important for organizations and businesses).
- You can track which software was installed and when — useful for troubleshooting.

---

**WHO does it?**

- IT technicians and system administrators in schools, offices, and businesses.
- Any responsible user who wants to keep track of their computer's health.
- Students learning computer maintenance (like you — right now).

---

**WHERE is it kept?**

- **Manually:** In a notebook, a spreadsheet, or a simple Word/Google Docs file.
- **Automatically:** Windows Event Viewer records logs automatically (as we learned in Section 2.2).
- **In organizations:** In dedicated IT management software or databases.

---

**WHEN do we document?**

- **Immediately after** every maintenance task — disk cleanup, update, virus scan.
- **Immediately after** fixing any problem — describe the problem and the solution.
- **When installing** any new software or hardware.
- **When an error occurs** — note the error message, the date, and what was done.

The key word is **immediately.** If you wait too long, you will forget the details.

---

**HOW do we document? — Creating a Maintenance Log**

A maintenance log does not need to be complicated. It just needs to be **consistent.**

Here is a simple template for a maintenance log entry:

| Field | Example Entry |
|---|---|
| **Date** | 4 June 2026 |
| **Computer / Device Name** | Lab Computer #12 / Student HP Laptop |
| **Task Performed** | Disk Cleanup, Windows Update, Full Virus Scan |
| **Problem Found (if any)** | 3 virus threats detected by Windows Defender |
| **Action Taken** | Threats quarantined and removed. Windows Defender updated. |
| **Result** | System running normally. No threats remaining. |
| **Next Scheduled Maintenance** | 4 July 2026 |
| **Technician / Person Name** | [Your Name] |

This can be written in a notebook, a spreadsheet, or even a simple text document. The format does not matter as much as the **habit** of writing it.

---

### 🛠️ Practical Walkthrough: Reading Windows Event Viewer Logs

Windows keeps its own automatic log in the **Event Viewer** (which we introduced in Section 2.2). Here is how to find and read useful information from it:

**Step by Step — Reading Event Viewer:**

- **Step 1:** Press **Windows key + R.** Type **`eventvwr`** and press **Enter.**
- **Step 2:** Event Viewer opens. On the left side, you see a folder tree.
- **Step 3:** Expand **"Windows Logs"** by clicking the arrow next to it.
- **Step 4:** Click on **"System"** — this shows events related to Windows itself (startup, shutdown, driver issues, hardware problems).
- **Step 5:** Click on **"Application"** — this shows events related to programs (crashes, errors in software).
- **Step 6:** In the middle panel, you will see a list of events with:
  - **Level:** Error (red), Warning (yellow), or Information (blue).
  - **Date and Time:** Exactly when it happened.
  - **Source:** Which part of Windows or which program caused the event.
  - **Event ID:** A specific number that identifies the type of event. You can search this number online to understand exactly what it means.
- **Step 7:** Click on any event to see its full details in the lower panel.

**Practical use:** If your computer crashed yesterday at 10:30 PM, open Event Viewer, filter the System logs for that time, and look for red "Error" events. The description and Event ID will tell you exactly what caused the crash.

---

### 🛠️ Your Final Task: Creating a Personal System Documentation File

Let us create your own maintenance record right now.

**Step 1:** Open a blank document on your computer (Word, Notepad, or Google Docs).

**Step 2:** Create a table with these column headers:

*Date | Computer Name | Task Done | Problem Found | Action Taken | Result | Next Due Date | Done By*

**Step 3:** Fill in your first entry based on what you did today in class — even if it was just opening Task Manager and checking system performance.

**Step 4:** Save the file with the name: **"Maintenance_Log_[YourName].docx"**

**Step 5:** Commit to adding to this log every time you perform maintenance on a computer — at school or at home. In six months, you will have a professional, organized history of everything you have done.

---

### 💡 Final Pause & Think — Stop Point #7

> **The Big Challenge — Putting It All Together:**
>
> A friend says to you: *"My computer has been crashing a lot lately. It started after I installed a new game last week. Also, it's been really slow, and I noticed the hard drive is almost full. I haven't updated Windows in months. And I have no idea what I did to it last year when it had a similar problem."*
>
> Based on everything you learned in this chapter, write a **complete action plan** for your friend. Include:
>
> 1. Which diagnostic tool would you open first, and what would you look for?
> 2. Which recovery option would help with the crashing caused by the new game?
> 3. Which maintenance task would you perform to address the slow speed and full hard drive?
> 4. How would you protect the system going forward?
> 5. What document would you create so that next time a similar problem happens, you have a record to look back at?
>
> Write at least **one full paragraph** for each point. Then share your plan with the class.

---

## 📚 Chapter Summary

Congratulations. You have completed one of the most practical chapters in all of Computer Science.

Here is what you now know:

| Section | Key Takeaway |
|---|---|
| **2.1 Post-Troubleshooting** | Fixing a problem is only the first step. Regular care prevents problems from returning. |
| **2.2 Diagnostic Tools** | Task Manager, Resource Monitor, and Event Viewer are your computer's cockpit — they show you exactly what is happening inside. |
| **2.3 System Recovery** | Safe Mode, System Restore, and Bootable Media are your safety net when things go seriously wrong. |
| **2.4 BIOS/UEFI** | Every computer starts with a hidden check (POST). BIOS/UEFI controls the boot process and can be adjusted when needed. |
| **2.5 Data Recovery** | Deleted files can often be recovered — but speed matters. Check the Recycle Bin first. Use Tenorshare for deeper recovery. |
| **2.6 Preventive Maintenance** | Disk Cleanup, software updates, and virus scans done regularly prevent disasters before they happen. |
| **2.7 Documentation & Logs** | Writing down what you do creates a history that helps everyone — including future you — manage systems better. |

---

> **One Final Thought:**
>
> Every skill in this chapter is a skill used by real professionals every single day. System administrators. IT helpdesk staff. Network engineers. Cybersecurity analysts. They all use these exact tools and techniques.
>
> You are not just studying for an exam. You are building a foundation for a career, a hobby, and a life skill that will be useful for as long as computers exist — which is likely to be a very long time.
>
> Well done. Keep going.

---

*End of Chapter 2 — System Recovery and Advanced Maintenance*
