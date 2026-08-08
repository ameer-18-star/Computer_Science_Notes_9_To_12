# Chapter 1: Computer Networks

*A CS50-style guide to how devices talk to each other*

Welcome. By the time you finish this chapter, you won't just know what a "network" is — you'll be able to look at your home Wi-Fi, your phone, or a school computer lab, and actually explain what's happening underneath. That's the goal: not memorization, but real understanding you can use.

Let's get into it.

---

## 1.1 Introduction to Computer Networks

### The Hook (Story Mode)

On October 29, 1969, a UCLA student named Charley Kline sat down to send the very first message over a brand-new experimental network called **ARPANET**, to a computer at Stanford, 560 kilometers away. He typed the word `LOGIN`. He got as far as **"L"**, then **"O"**... and then the whole system crashed.

That's it. The first message ever sent over a computer network was "LO" — as in "Lo and behold." An hour later, engineers fixed the bug, and the full message went through. That clumsy, half-broken first attempt was the beginning of everything you now call the Internet.

The lesson? Every network you use today — Wi-Fi, mobile data, YouTube, Discord — grew out of two university computers barely managing to say hello to each other. Networking is, at its core, just getting devices to say "hello" reliably.

### The Explanation

A **computer network** is a group of two or more devices connected together so they can share data and resources. "Devices" doesn't just mean computers — it means phones, printers, smart TVs, game consoles, even your smart fridge.

Think about what you did in the last hour. You probably:

* Sent a WhatsApp message (your phone talked to a server, which talked to your friend's phone)
* Streamed a video (a server somewhere sent you millions of tiny pieces of data)
* Maybe printed a document from your laptop to a printer down the hall

All of that is networking. Without networks, every device would be an island — powerful on its own, but unable to share anything with anyone.

**Why do networks matter?**

* They save time. You don't have to walk a USB drive to your friend's house to share a photo.
* They save money. One printer can serve an entire office instead of buying one printer per desk.
* They enable things that are *impossible* alone — like a video call, where two cameras and two microphones must exchange data continuously, in real time.

### Uses of Computer Networks

* **Internet browsing** — loading websites, search engines, and apps.
* **Communication** — calls, texts, video chat, email.
* **Education** — online classes, learning management systems, digital libraries.
* **Banking** — ATMs, mobile banking apps, online transfers.
* **Social media** — Instagram, TikTok, Facebook all run over networks connecting billions of devices.
* **Smart homes** — smart bulbs, cameras, and thermostats controlled from an app.

> **TIDBIT**
> Networks quietly power things you don't think about as "networking" at all — traffic lights that talk to each other, hospital equipment sharing patient vitals, and even your car's GPS pulling live map data.

### The Practical Walkthrough

Let's trace what happens, in plain terms, when you send one WhatsApp message:

| Step | What happens |
|---|---|
| 1 | You type "Hey!" and hit send on your phone. |
| 2 | Your phone breaks the message into small chunks of data. |
| 3 | Your phone sends those chunks over Wi-Fi or mobile data to a nearby network device. |
| 4 | The chunks travel across many connected networks (this *is* the Internet) toward WhatsApp's servers. |
| 5 | The server figures out which device your friend is using and forwards the chunks there. |
| 6 | Your friend's phone receives the chunks and reassembles them into "Hey!" |

**What just happened?** A message that felt instant actually traveled through several devices and networks in a fraction of a second. That's the power — and the invisible complexity — of networking.

### Interactive Stop-Point

**Pause & Think:** List 5 things you did today that relied on a computer network, without you consciously thinking "I am using a network right now." For each one, guess: was it wired, wireless, or both?

### Quick Recap

A computer network connects devices so they can share data quickly, cheaply, and reliably — and it's already invisibly present in almost everything you do each day.

---

## 1.2 Network Architecture and Basic Concepts

### The Hook (Story Mode)

Imagine designing a city from scratch. You wouldn't just drop houses randomly — you'd plan roads, intersections, traffic rules, and address systems so mail and cars could actually reach the right places. **Network architecture** is that same city-planning exercise, but for data.

### The Explanation

**Network architecture** is the overall design of a network — how devices are arranged, how they're connected, and what rules govern how data moves between them. It includes three ingredients working together:

* **Hardware** — cables, routers, switches, the physical "roads."
* **Software** — the programs and operating systems that manage traffic.
* **Communication rules (protocols)** — the "traffic laws" that keep everything orderly.

A good architecture is like a well-planned city: it handles current traffic smoothly and still has room to grow when the city (or the network) gets bigger.

```
        [ Laptop ]      [ Phone ]
             \             /
              \           /
             [   Router/Switch  ]
                     |
              [   Modem   ]
                     |
              [  Internet  ]
                     |
        [ Websites, Servers, Cloud ]
```

This is a simplified **network architecture diagram**. Notice how devices don't talk directly to "the Internet" — they go through layers of local hardware first.

### The Practical Walkthrough

How data actually travels, step by step:

1. Your device creates data (a message, a video request, a game move).
2. The data is broken into small pieces called **packets**.
3. Each packet gets a "destination label" (an IP address, covered in 1.8).
4. Networking devices (routers, switches) read the label and forward the packet toward its destination — hop by hop, like mail passing through sorting offices.
5. At the destination, packets are reassembled into the original data, in the correct order.

**What just happened?** Instead of sending one giant blob of data in one shot, the network splits it into manageable, independently-routable pieces. If one packet gets lost or delayed, only that piece needs to be resent — not the whole message.

### Interactive Stop-Point

**Pause & Think:** Why do you think engineers chose to break data into small packets instead of sending everything as one big continuous stream? What could go wrong with one giant stream if the connection briefly drops?

### Quick Recap

Network architecture is the blueprint of a network — hardware, software, and protocols working together so data can travel efficiently, in small routable packets, from source to destination.

---

## 1.3 Types of Computer Networks

### The Hook (Story Mode)

Picture three circles of communication in your life: the people in your house (small, fast, easy), the people in your city or country (bigger, slower to reach), and literally anyone on Earth with an Internet connection (huge, global). Computer networks are classified the exact same way — by how much ground they cover.

### The Explanation

Networks are grouped mainly by **size and coverage area**.

**Local Area Network (LAN)**

A LAN connects devices within a small area — a home, a classroom, a single office building. It's fast, cheap, and usually owned and managed by one person or organization (you, or your school's IT department). Most LANs today use Ethernet cables and Wi-Fi.

```
   [PC 1] --\
   [PC 2] ---+--- [ Switch ] --- [ Router ] --- Internet
   [PC 3] --/
        (All inside one building = LAN)
```

**Wide Area Network (WAN)**

A WAN connects networks across a large geographic area — different cities or even different countries. WANs use leased telecom lines, satellites, or the Internet itself to link distant LANs together. They're slower and more expensive to build than LANs because the distances are so much greater.

**The Internet (Public WAN)**

The Internet is the biggest WAN of all — a global network of networks connecting billions of devices. No single company owns it. It runs on standardized protocols so that a phone in Lahore and a server in California can understand each other perfectly.

> **DO YOU KNOW?**
> **ISP (Internet Service Provider):** the company that connects your home or business to the wider Internet (like a local road connecting your house to the national highway system).
> **DSL (Digital Subscriber Line):** a technology that delivers Internet over ordinary telephone lines, letting you browse and make calls at the same time.

### The Practical Walkthrough

Let's compare all three side by side:

| Feature | LAN | WAN | Internet |
|---|---|---|---|
| Coverage | One building/campus | Cities/countries | Global |
| Speed | Very high | Lower (distance-limited) | Varies |
| Cost | Low | High | Shared, built on WAN tech |
| Ownership | Single organization | Multiple organizations | No single owner |
| Example | School computer lab | A bank's branches nationwide | YouTube, Google, WhatsApp |

**What just happened?** You now have a mental map: LAN = your room, WAN = your whole country's road network, Internet = the entire planet's road network connected together.

### Interactive Stop-Point

**Grab a Partner:** With a partner, list every network you're personally connected to right now (school Wi-Fi, mobile data, home Wi-Fi at another time of day). Classify each as LAN or part of a WAN, and explain why.

### Quick Recap

LAN covers a small local space, WAN stretches across cities or countries, and the Internet is the largest public WAN — a global network connecting virtually everyone.

---

## 1.4 Networking Devices

### The Hook (Story Mode)

Every character in a heist movie has a job: the driver, the safecracker, the lookout. Networking devices work the same way — each one has one specific job, and the network only works when all of them play their role correctly.

### The Explanation

**Network Interface Card (NIC)**

The NIC is what lets a device physically join a network — wired or wireless. Every NIC has a unique **MAC address**, a built-in "serial number" used to identify the device on a local network. No NIC, no networking — it's the device's passport.

**Switch**

A switch connects multiple devices *within* the same LAN and uses MAC addresses to send data only to the correct device — not to everyone. Think of a switch as an **office intercom system**: when you page one specific desk, only that desk's phone rings, not the whole building.

**Router**

A router connects *different* networks to each other — most commonly, your home LAN to the wider Internet. It reads IP addresses (not MAC addresses) and decides the best path to send data. Think of a router as an **international airport**: it doesn't care about your local neighborhood — its job is to connect entire cities (networks) to each other.

**Modem**

A modem connects your local network to your ISP. It converts your device's digital data (1s and 0s) into signals that can travel over cable, DSL, or fiber lines — and converts incoming signals back into digital data. No modem, no Internet access, regardless of how good your router is.

**Wireless Access Point (WAP)**

A WAP broadcasts a Wi-Fi signal so wireless devices can join the network without cables. It's especially useful in large buildings or campuses where one router's signal alone wouldn't reach every corner.

```
[ISP] --- [Modem] --- [Router] --- [Switch] --- [Wired PCs]
                          |
                    [Wireless AP]
                          |
                [Phones, Laptops, Tablets]
```

### The Practical Walkthrough

A quick "who does what" decision table:

| You want to... | Device responsible |
|---|---|
| Let your laptop physically join a network | NIC |
| Connect 5 office desktops together | Switch |
| Connect your home network to the whole Internet | Router |
| Convert your ISP's signal into digital data | Modem |
| Add Wi-Fi coverage to a big building | Wireless Access Point |

**What just happened?** You just built, on paper, the exact chain of devices your data passes through every time you open a website at home: device → NIC → switch/AP → router → modem → ISP → Internet.

### Interactive Stop-Point

**Pause & Think:** Your Wi-Fi shows "connected" but you still can't load any websites. Which device is most likely at fault — the router, the modem, or the switch? Explain your reasoning.

### Quick Recap

NICs let devices join a network, switches connect devices *within* one network using MAC addresses, routers connect *separate* networks using IP addresses, modems translate signals for your ISP, and access points spread Wi-Fi coverage.

---

## 1.5 Network Topologies

### The Hook (Story Mode)

Imagine you're seating five friends at a birthday party. You could seat them in a straight line (one long table), around a single host in the middle (a round table with you at the head), or in a full circle where everyone can pass food to their neighbor. Each seating arrangement changes how quickly a message travels around the table, and what happens if one seat is empty. That's exactly what a **network topology** is — the seating arrangement for your devices.

### The Explanation

A **topology** is the layout of a network — how devices and cables are physically or logically arranged. **Physical topology** is the actual wiring you'd see if you opened the walls. **Logical topology** is the path data actually flows, which isn't always the same as the physical layout.

**Bus Topology**

```
Device1---Device2---Device3---Device4---Device5
        (single shared cable, "the bus")
```
All devices share one central cable. Simple and cheap, but if the main cable breaks, the *entire* network goes down. Good for small, non-critical networks only.

**Star Topology**

```
        Device1
           |
Device2--[Switch/Hub]--Device3
           |
        Device4
```
All devices connect to one central hub or switch. If one device's cable fails, only that device drops off — everyone else keeps working. But if the central hub fails, the *whole* network dies. This is the most common topology in modern homes and offices.

**Ring Topology**

```
Device1---Device2
   |          |
Device4---Device3
(data travels in one direction around the ring)
```
Devices form a closed loop; data passes from device to device in one direction. It's more organized (no data collisions) but if one device or link fails, it can break the entire ring. Rarely used today.

**Mesh Topology**

```
Device1---Device2
  |   \   /   |
  |    \ /    |
Device4---Device3
(many direct connections between devices)
```
Every device connects to many other devices, creating multiple possible paths. If one link fails, data simply reroutes. Extremely reliable, but expensive and complex to wire — used mainly in critical systems like military or backbone Internet infrastructure.

**Tree Topology**

```
                [Backbone/Server]
               /        |        \
         [Hub 1]     [Hub 2]    [Hub 3]
          /  \         /  \        /  \
        PC  PC       PC  PC     PC   PC
```
A hierarchical mix of star networks connected to one backbone — like the branches of a real tree. Easy to expand for large organizations, but if the backbone fails, everything below it loses connection.

### Advantages and Disadvantages of Network Topologies

| Topology | Advantages | Disadvantages |
|---|---|---|
| Bus | Simple, cheap, less cable | Whole network fails if main cable breaks; hard to troubleshoot |
| Star | Easy to manage; one device failing doesn't affect others | Central hub failure kills the whole network; more cable needed |
| Ring | Organized data flow, no collisions | One failure can break the entire ring; rarely used today |
| Mesh | Extremely reliable; multiple paths | Very expensive; complex to install and wire |
| Tree | Easy to expand; good for large organizations | Backbone failure affects everything below it |

### The Practical Walkthrough

Let's stress-test each topology with the same failure scenario: **one cable breaks.**

| Topology | What happens when ONE cable breaks |
|---|---|
| Bus | Entire network goes down — the shared cable is gone. |
| Star | Only the one disconnected device is affected; everyone else is fine. |
| Ring | The ring is broken; data can't complete its loop, and connectivity is disrupted. |
| Mesh | Almost nothing happens — data reroutes through another path automatically. |
| Tree | Depends on *which* cable — a branch cable affects only that branch; the backbone cable affects everyone below it. |

**What just happened?** You just performed a basic **fault-tolerance analysis** — exactly the kind of thinking real network engineers do before choosing a topology for a hospital, a bank, or a gaming café.

### Interactive Stop-Point

**Pause & Think:** If you were designing the network for a hospital's ICU (where losing connectivity could be life-threatening), which topology would you pick, and why? What would you accept in extra cost or complexity to get that reliability?

### Quick Recap

A topology is the wiring "seating plan" of a network — star is the most common and forgiving choice today, mesh is the most reliable but costly, and bus/ring are largely historical due to their single-point-of-failure weaknesses.

---
## 1.6 Network Models and Layers

### The Hook (Story Mode)

Imagine writing a birthday card for a friend in another city. You write the message (the fun part), put it in an envelope with an address (so the post office knows where it's going), hand it to a mail carrier (who doesn't read your message, just moves the envelope), and it travels down real roads to reach your friend. Each step is handled by a different "layer" of the postal system, and none of them need to understand what the others are doing. That's precisely the idea behind network layers.

### The Explanation

Real reassurance first: **the OSI model confuses even senior network engineers when they first meet it.** It is not physical hardware you can touch — it's a conceptual map that organizes an incredibly complex process (getting data from Point A to Point B) into manageable, independent stages.

**Network Layers**

A network layer is one stage in the journey of data, with one specific job. Data passes through these stages one after another. Because each layer is independent, engineers can change or fix one layer (say, upgrading Wi-Fi hardware) without having to redesign everything else (like the apps running on top of it).

**The OSI Model (Open Systems Interconnection)**

The OSI model is the standard 7-layer reference model used to understand and design network communication.

```
SENDER SIDE                          RECEIVER SIDE
+-------------+                      +-------------+
| Application |  <-- data created    | Application |  <-- data delivered
+-------------+                      +-------------+
| Presentation|                      | Presentation|
+-------------+                      +-------------+
|  Session    |                      |  Session    |
+-------------+                      +-------------+
|  Transport  |                      |  Transport  |
+-------------+                      +-------------+
|  Network    |                      |  Network    |
+-------------+                      +-------------+
|  Data Link  |                      |  Data Link  |
+-------------+                      +-------------+
|  Physical   |  --> signal sent --> |  Physical   |
+-------------+                      +-------------+
```

### Functions of OSI Model Layers

1. **Physical Layer** — Sends raw bits as electrical, light, or radio signals. Defines cables, connectors, and voltage levels. (*Link:* This is the actual Wi-Fi radio wave carrying your Instagram scroll.)
2. **Data Link Layer** — Ensures error-free transfer between two directly connected devices; handles MAC addressing and framing. (*Link:* This is how your laptop and router recognize each other on the same Wi-Fi.)
3. **Network Layer** — Handles logical addressing (IP addresses) and picks the best route across networks. (*Link:* This decides whether your data goes through your ISP in Islamabad or a data center abroad.)
4. **Transport Layer** — Ensures reliable, ordered delivery; breaks data into segments, and can request re-sends of lost pieces. (*Link:* This is why a video call doesn't play your words out of order.)
5. **Session Layer** — Opens, manages, and closes a communication "session" between two apps. (*Link:* This is why your Zoom call stays connected as one continuous session instead of reconnecting every second.)
6. **Presentation Layer** — Formats, encrypts, and compresses data so both ends understand it the same way. (*Link:* This is why an HTTPS website looks the same whether you're on Chrome or Safari.)
7. **Application Layer** — The layer closest to you — the actual apps and protocols like HTTP, email, and file transfer. (*Link:* This is the "Send" button you click in WhatsApp.)

> **TIDBIT**
> Lower layers (1–2) move raw signals. Middle layers (3–4) handle addressing and reliable delivery. Upper layers (5–7) support the actual applications you interact with. Each layer only needs to trust the layer directly below it — it doesn't need to understand everything happening underneath.

### The Practical Walkthrough: Tracing an HTTP Request Down and Up the OSI Stack

Let's trace what happens when your browser requests a webpage, layer by layer, on the **sender's** side (**encapsulation** — wrapping data in extra info at each layer):

| Layer | What gets added | Plain-language meaning |
|---|---|---|
| 7. Application | HTTP request ("GET /index.html") | "I want this webpage" |
| 6. Presentation | Encryption/formatting (if HTTPS) | "Scramble this so only the server can read it" |
| 5. Session | Session ID | "This is part of an ongoing conversation with the server" |
| 4. Transport | TCP header (port numbers, sequence number) | "This chunk is piece #4 of the total request" |
| 3. Network | IP header (source & destination IP) | "This is going to 93.184.216.34" |
| 2. Data Link | MAC header (source & destination MAC) | "Hand this to the router's network card next" |
| 1. Physical | Raw bits as electrical/radio signal | "Here's the actual electrical pulse" |

At the receiving server, the exact reverse happens — this is called **decapsulation**: each layer strips off its own header, reads the instructions meant for it, and passes the rest upward, until the raw HTTP request reaches the web server's application layer.

**What just happened?** Your single click on a link triggered seven mini-translations, each adding just enough information for the next device to know what to do — without any single layer needing to understand the whole picture.

### Interactive Stop-Point

**Pause & Think:** If the Transport layer's job is to guarantee reliable, ordered delivery, what do you think would happen to a video call if this layer didn't exist? Would frames arrive out of order? Would some frames get lost with no way to notice?

### Quick Recap

The OSI model splits data communication into 7 independent layers — from raw physical signals up to the applications you use — so complexity is manageable, changeable, and easier to troubleshoot.

---

## 1.7 Network Protocols and Services

### The Hook (Story Mode)

Protocols are like languages computers use to talk to each other. Imagine two diplomats from different countries meeting: if they don't agree on a shared language and etiquette beforehand, the meeting fails immediately — no matter how good the message is. Networking protocols are that shared, pre-agreed language.

### The Explanation

A **network protocol** is a set of rules defining how data is formatted, sent, and understood. Every device on a network must follow the *same* protocol to communicate — just like both diplomats must speak the same language.

**TCP/IP (Transmission Control Protocol / Internet Protocol)**

TCP/IP is the foundational protocol suite of the entire Internet.

* **IP** handles addressing and routing — it figures out *where* data should go.
* **TCP** handles reliability — it makes sure all the pieces *arrive completely and in order*, resending anything lost.

*Link:* Think of IP as writing the destination address on a package, and TCP as the delivery company that tracks every box, confirms delivery, and resends anything that got lost in transit.

**HTTP (Hypertext Transfer Protocol) and HTTPS**

HTTP is used to load web pages — it's the language your browser and a web server use to request and deliver content. Plain HTTP sends data **unencrypted**, meaning anyone snooping on the network could read it. **HTTPS** is the secure version: it uses **SSL/TLS encryption** to scramble the data in transit, so passwords, personal details, and payment information can't be easily intercepted.

*Link:* That little padlock icon in your browser bar? That's HTTPS quietly protecting your online banking session right now.

**FTP (File Transfer Protocol)**

FTP is used to upload and download files between computers — commonly used by web developers to publish files to a website's server. Secure versions (like FTPS or SFTP) add encryption for safety.

**DNS (Domain Name System)**

DNS converts human-friendly website names (like `google.com`) into the numeric IP addresses computers actually use (like `142.250.190.14`). Without DNS, you'd have to memorize a string of numbers for every website you want to visit.

*Link:* DNS works exactly like the Contacts app on your phone — you tap "Mom," but your phone actually dials her 10-digit number behind the scenes. You never have to remember the number yourself.

### The Practical Walkthrough: DNS Resolution Step-by-Step

Let's trace what happens the instant you type `example.com` into your browser and hit Enter:

| Step | What happens | Plain meaning |
|---|---|---|
| 1 | Browser checks its own **cache** | "Have I already looked this up recently?" |
| 2 | If not found, it asks the **Local DNS Resolver** (usually run by your ISP) | "Do you already know this address?" |
| 3 | If the resolver doesn't know, it asks a **Root Server** | "Who handles `.com` addresses?" |
| 4 | Root Server points to a **TLD (Top-Level Domain) Server** for `.com` | "Ask the `.com` server next." |
| 5 | TLD Server points to the **Authoritative Server** for `example.com` | "This specific server knows the real answer." |
| 6 | Authoritative Server replies with the actual IP address | "`example.com` = `93.184.216.34`" |
| 7 | Your browser finally sends the real HTTP request to that IP address | The webpage starts loading |

**What just happened?** A process that feels instant actually involved up to 5–6 different servers around the world, all consulted in a fraction of a second, just to translate one readable name into the number your computer actually needs.

### Interactive Stop-Point

**Grab a Partner:** Open a terminal and run `nslookup google.com` (or ask your partner to). Compare the IP addresses you each get back. Are they identical? Discuss why large companies might return *different* IP addresses to users in different locations.

### Quick Recap

Protocols are the shared rulebooks that let devices communicate — TCP/IP moves and delivers data reliably, HTTP(S) loads webpages securely, FTP transfers files, and DNS quietly translates readable names into the IP addresses machines actually use.

---

## 1.8 IP Addressing and Subnetting

### The Hook (Story Mode)

In the late 1970s, Vint Cerf and Bob Kahn designed IPv4 with 32-bit addresses, giving the world about 4.3 billion possible unique addresses. At the time, that number seemed almost limitless — "more than humanity could ever need." Fast forward to today: with billions of phones, laptops, smart bulbs, and fitness trackers, IPv4 has technically run out of fresh addresses. This crunch is exactly why IPv6 — with a mind-bendingly larger address space — had to be invented.

### The Explanation

An **IP address** is a unique number assigned to a device so it can be identified and reached on a network. Just like a home address lets mail find your house, an IP address lets data find your device.

**IPv4**

IPv4 addresses are 32 bits long, written as four numbers (0–255) separated by dots — for example, `192.168.1.10`. Each of the four numbers is one **byte** (8 bits), and 4 bytes × 8 bits = 32 bits total.

```
192   .  168  .  1    .  10
--- 8 bits each, 4 groups = 32 bits total ---
```

| Part | Example value | Plain meaning |
|---|---|---|
| Network part | 192.168.1 | Identifies your local network — like "Gulshan Block Street 3" |
| Host part | 10 | Identifies your specific device on that network — like "House #10" |

> **DO YOU KNOW?** Total possible IPv4 addresses: about **4.29 billion**. That sounds huge — until you remember there are over 8 billion people on Earth, many with 3+ connected devices each.

**IPv6**

IPv6 addresses are 128 bits long, written as 8 groups of 4 hexadecimal digits separated by colons — for example, `2001:0db8:0000:0000:0000:ff00:0042:8329`. Each group is 16 bits, and 8 groups × 16 bits = 128 bits total.

| Part | Example value | Plain meaning |
|---|---|---|
| Global routing prefix | 2001:0db8 | Identifies the ISP/region — like "Pakistan, Sindh, Karachi" |
| Subnet ID | 0000 | Identifies your local network inside the ISP — like "Gulshan area" |
| Interface ID | 0000:ff00:0042:8329 | Identifies your specific device — like "your exact house" |

> **DO YOU KNOW?** IPv6 supports approximately **340 undecillion** addresses (3.4 × 10^38). That number is so large it will realistically never run out — there are enough IPv6 addresses to assign one to every grain of sand on Earth, many times over.

**Subnetting**

Subnetting divides one large network into smaller, more manageable pieces called **subnets**. This reduces unnecessary traffic, improves performance, and increases security by isolating groups of devices from each other.

```
192.168.1.0/24  (one big network — 256 addresses)
        |
        +--- Subnet 1: 192.168.1.0/25   (first half — 128 addresses)
        +--- Subnet 2: 192.168.1.128/25 (second half — 128 addresses)
```

**Network Address Translation (NAT)**

NAT lets many devices inside a home or office share a single public IP address when talking to the outside Internet. Your router performs NAT automatically: your laptop, phone, and smart TV all have private IP addresses at home, but to the outside world, they all appear to be coming from one shared public address. This hides your internal devices from the Internet, which is a real security benefit.

### The Practical Walkthrough: Subnetting `192.168.1.0/24` Step by Step

Let's actually split a real network. Starting network: **`192.168.1.0/24`** (the `/24` means the first 24 bits are the fixed "network part," leaving 8 bits free for hosts).

**Step 1 — Understand the starting point.**
`/24` = 24 network bits + 8 host bits = 2^8 = 256 total addresses (192.168.1.0 through 192.168.1.255).

**Step 2 — Decide how many subnets you need.**
Let's say we want 2 equal subnets. We "borrow" 1 bit from the host part, making it `/25` (25 network bits + 7 host bits).

**Step 3 — Calculate addresses per subnet.**
2^7 = 128 addresses per subnet.

**Step 4 — Write out both subnets.**

| Subnet | Network Address | Usable Host Range | Broadcast Address |
|---|---|---|---|
| Subnet 1 | 192.168.1.0 | 192.168.1.1 – 192.168.1.126 | 192.168.1.127 |
| Subnet 2 | 192.168.1.128 | 192.168.1.129 – 192.168.1.254 | 192.168.1.255 |

**Step 5 — Understand what each address means.**
* The **network address** (first address) identifies the subnet itself — it's never assigned to a device.
* The **broadcast address** (last address) is used to send a message to *every* device on that subnet at once — it's also never assigned to a single device.
* Everything in between is a **usable host address** — these are the ones actually assigned to laptops, phones, printers, etc.

**What just happened?** You just split one 256-address network into two clean, independent 128-address subnets — a real skill used by network administrators to organize company departments (e.g., "HR gets Subnet 1, Engineering gets Subnet 2") without buying any new hardware.

### Interactive Stop-Point

**Pause & Think:** If `192.168.1.0/24` has 256 total addresses, and you split it into 4 equal subnets instead of 2, how many addresses would each subnet have? (Hint: how many bits would you need to borrow this time?)

*(Answer: borrowing 2 bits gives you 2^2 = 4 subnets, each with 2^6 = 64 addresses.)*

Getting subnet math wrong on your first few tries is completely normal — it's practically a rite of passage every network engineer goes through. Keep practicing with small examples until the binary "clicks."

### Quick Recap

IPv4 uses 32-bit addresses (about 4.3 billion, now scarce), IPv6 uses 128-bit addresses (essentially inexhaustible), subnetting splits one network into smaller manageable pieces, and NAT lets a whole household share just one public IP address.

---

## 1.9 Home Network Setup and Configuration

### The Hook (Story Mode)

Think about the last time you set up a new Wi-Fi router at home — even if it was your parents who did it. Within a few minutes, a plastic box on your shelf became the reason your phone, laptop, and smart TV could all talk to each other *and* to the entire Internet. That's a home network — one of the most common real-world networks you'll ever personally configure.

### The Explanation

A **home network** connects the various devices in a house so they can share one Internet connection and communicate with each other (e.g., printing from your laptop to a wireless printer).

**Components of a Home Network**

* **Router** — the central traffic director for all devices in the home.
* **Modem** — connects the home network to the ISP.
* **End devices** — computers, laptops, phones, smart TVs, game consoles.
* **Cables** — for wired connections (Ethernet).
* **Wireless signals** — Wi-Fi, for devices without cables.

**Wired Network Connections**

Wired connections use Ethernet cables to connect devices directly to a router or switch. They're fast, stable, and more secure — but devices can't move freely since they're tied down by a physical cable. Great for gaming PCs, desktops, or smart TVs that never move.

**Wireless Network Connections**

Wireless connections use radio signals (Wi-Fi) instead of cables. Devices can move freely anywhere within range, and setup is simple — but wireless can be slower or less stable than wired, especially with walls, distance, or interference from other devices.

### The Practical Walkthrough

Comparing both connection types side by side:

| Feature | Wired (Ethernet) | Wireless (Wi-Fi) |
|---|---|---|
| Speed | Very high, stable | Can vary with distance/interference |
| Mobility | None — tied to a cable | Full freedom of movement |
| Security | Harder to intercept | Needs strong encryption (see 1.10) |
| Setup difficulty | Simple, plug-and-play | Simple, but needs password configuration |
| Best for | Gaming PCs, desktops, servers | Phones, laptops, tablets |

**What just happened?** You've just made the same trade-off decision every home network setup requires: prioritize raw speed and stability (wired) or freedom and convenience (wireless) — most homes today use *both*, choosing wisely per device.

### Interactive Stop-Point

**Pause & Think:** Your family has one gaming console for competitive online gaming, and three phones for browsing. Which devices would you connect via Ethernet, and which via Wi-Fi? Justify your choice using the table above.

### Quick Recap

A home network combines a router, modem, and various devices — wired connections trade mobility for speed and stability, while wireless connections trade some speed for full freedom of movement.

---

## 1.10 Wi-Fi Security and Router Configuration

### The Hook (Story Mode)

Imagine leaving your front door wide open in a busy neighborhood — anyone could walk in, take what they want, and you might never notice until it's too late. An unsecured Wi-Fi network is exactly that open door, except the "burglars" can be on the other side of the world, and what they're stealing is your personal data.

### The Explanation

**Wi-Fi security** protects your network from unauthorized access. Without it, strangers can use your internet, slow it down, or — much worse — intercept and steal personal information like passwords and messages.

**Router Web Interface**

Every router has a built-in web-based control panel, accessed by typing the router's IP address (often something like `192.168.1.1` or `192.168.0.1`) into a browser. Logging in (with a username and password — please change these from the factory defaults!) lets you change the Wi-Fi name, password, and security settings.

**Wi-Fi Encryption**

Encryption scrambles the data traveling over your Wi-Fi so outsiders can't read it, even if they intercept it. Modern routers should use **WPA2** or, ideally, **WPA3** — the newest and strongest standard. The old **WEP** standard is outdated and can be cracked in minutes; it should never be used today.

**Default Gateway**

The default gateway is the device (almost always your router) that connects your local network to outside networks. Any data leaving your home network for the wider Internet passes through the default gateway first — it's the "exit door" of your home network.

### Guest Networks

A guest network is a separate Wi-Fi network for visitors, isolated from your main home network. Guests can browse the Internet, but they can't see or access your personal devices, files, or smart home gadgets. This is a simple but powerful privacy and security habit — especially useful for homes with smart locks, cameras, or shared family computers.

### The Practical Walkthrough: Setting a Strong Router Password

1. Open a browser and type your router's IP address (check the label on the router, or run `ipconfig`/`ifconfig` — covered in 1.11 — to find the "Default Gateway").
2. Log in using the router's admin credentials (change these immediately if they're still the factory defaults like `admin`/`admin`).
3. Navigate to the wireless security settings.
4. Select **WPA3** (or WPA2 if WPA3 isn't available) as the encryption method.
5. Set a strong Wi-Fi password: at least 8 characters, mixing upper/lowercase letters, numbers, and symbols.
6. Enable a separate **Guest Network** for visitors, with its own distinct password.
7. Save and reboot the router.

**What just happened?** You just converted an "open door" network into a locked, monitored, and visitor-friendly home — the exact process real IT administrators follow when securing a new office router.

### Interactive Stop-Point

**Pause & Think:** Create a sample strong Wi-Fi password that is exactly 8 alphanumeric characters long and includes at least one uppercase letter, one number, and avoids obvious patterns (like `12345678` or your own name).

### Quick Recap

Wi-Fi security means using strong encryption (WPA2/WPA3), changing default router credentials, and offering a separate guest network — small habits that turn a wide-open home network into a genuinely protected one.

---

## 1.11 Network Diagnostic Tools and Commands

### The Hook (Story Mode)

Don't think of `ping` or `ipconfig` as scary "hacker tools." Think of them as flashlights. Your network is an invisible highway of data you can't normally see — these commands simply let you shine a light on it for a second, so you can understand what's actually happening instead of guessing.

### The Explanation

**Network diagnostic tools** help identify problems — slow connections, broken links, or misconfigured settings — by directly querying the network instead of guessing blindly.

**The Ping Command**

`ping` tests whether a device is reachable on the network, and measures how long the round trip takes.

```
Host A                              Host B
  |------ ICMP Echo Request  ------->|
  |<----- ICMP Echo Reply    --------|
```

Sample output:
```
ping google.com

Pinging google.com [142.250.190.14] with 32 bytes of data:
Reply from 142.250.190.14: bytes=32 time=25ms TTL=118
Reply from 142.250.190.14: bytes=32 time=24ms TTL=118
Reply from 142.250.190.14: bytes=32 time=26ms TTL=118
Reply from 142.250.190.14: bytes=32 time=25ms TTL=118
```

Reading this line by line:
* `bytes=32` — the size of the small test packet sent.
* `time=25ms` — the **round-trip time (RTT)** — how long it took for the reply to come back. Lower is better.
* `TTL=118` — **Time To Live**: a countdown value that prevents packets from looping forever if something goes wrong; it drops by 1 at every router hop.

**Ipconfig and Ifconfig Commands**

* `ipconfig` — used on **Windows** — displays your device's current network settings.
* `ifconfig` — used on **Linux and macOS** — does the same job on those systems.

Both show your IP address, subnet mask, and default gateway — essential information for troubleshooting connectivity.

**Telnet, PuTTY, and Secure Shell (SSH)**

* **Telnet** allows remote access to another device but sends everything — including passwords — completely unencrypted. It's outdated and unsafe for anything sensitive today.
* **PuTTY** is a popular free tool for remote login (often used with SSH on Windows).
* **SSH (Secure Shell)** is the modern, secure replacement for Telnet — it encrypts the entire session, so credentials and commands can't be intercepted.

### The Practical Walkthrough: Reading an `ipconfig` Output

```
ipconfig

Wireless LAN adapter Wi-Fi:
   IPv4 Address. . . . . . . . . . . : 192.168.1.15
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . : 192.168.1.1
```

| Line | Plain meaning |
|---|---|
| IPv4 Address: 192.168.1.15 | This is *your* device's private address on the home network. |
| Subnet Mask: 255.255.255.0 | This tells your device which part of the address is the "network" and which part is the "host" (matches a `/24` network, as in 1.8). |
| Default Gateway: 192.168.1.1 | This is your router — the exit point to reach the Internet. |

**What just happened?** In under 2 seconds, you extracted the exact 3 pieces of information (your address, your network boundary, and your exit point) that 90% of home network troubleshooting depends on.

### Interactive Stop-Point

**Grab a Partner:** Run `ping 8.8.8.8` on your own computer (this is one of Google's public DNS servers). Compare your average response time (in ms) with your partner's — even if you're on the exact same Wi-Fi network. Discuss at least two possible reasons your numbers might differ (distance from the access point, background downloads, device hardware, etc.).

### Quick Recap

`ping` tests reachability and speed, `ipconfig`/`ifconfig` reveal your device's core network settings, and SSH has replaced the old, insecure Telnet as the safe standard for remote device access.

---
## 1.12 Network Performance

### The Hook (Story Mode)

Picture a highway. **Bandwidth** is how many lanes the highway has — more lanes mean more cars (data) can travel at the same time. **Latency** is the speed limit — how long it takes one single car to complete the trip, regardless of how many other lanes exist. A highway can have 10 lanes (huge bandwidth) but still have a low speed limit through a mountain pass (high latency). Both matter, but they measure completely different things.

### The Explanation

**Network performance** describes how well a network works — its speed and the quality of data transfer.

**Network Bandwidth**

Bandwidth is the *amount* of data a network can carry in a given time, usually measured in **Mbps (megabits per second)**. Higher bandwidth means more data can move at once — useful when many devices are active simultaneously (e.g., one person streaming 4K video while another is on a video call).

**Network Latency**

Latency is the *delay* between sending data and receiving a response, measured in **milliseconds (ms)**. Low latency means a near-instant response — critical for online gaming and video calls, where even small delays are noticeable and frustrating.

*Link:* This is why a fast Wi-Fi connection (high bandwidth) can still feel "laggy" in a competitive game (high latency) — bandwidth and latency are simply not the same thing.

**Causes of Network Delay**

* Too many users competing for the same connection.
* Poor-quality or damaged cables.
* Long physical distance between communicating devices.
* Network congestion (too much traffic at once).
* Hardware problems (old routers, failing switches).

### The Practical Walkthrough

Let's compare two real scenarios:

| Scenario | Bandwidth | Latency | Real Result |
|---|---|---|---|
| Downloading a large movie file | High (needed) | Doesn't matter much | Fast download, no annoyance if latency is a bit high |
| Playing a competitive online shooter | Doesn't need to be huge | Must be very low | A "laggy" connection ruins gameplay even with fast bandwidth |
| Video call with 10 participants | High (needed for many video streams) | Must be low (needed for real-time voice) | Both matter equally — the hardest scenario to get right |

**What just happened?** You just diagnosed why "my Wi-Fi shows full bars but my game still lags" is a completely valid and common complaint — full signal strength affects bandwidth, not necessarily latency.

### Interactive Stop-Point

**Pause & Think:** Identify the likely cause of delay in this scenario: A family of 6 is all using the same home Wi-Fi at 8 PM — two are streaming Netflix in HD, one is gaming online, and three are on video calls for school/work, all at once. What's happening, and what would you recommend?

### Quick Recap

Bandwidth measures *how much* data can move at once, while latency measures *how fast* a single piece of data makes the round trip — great network performance requires managing both.

---

## 1.13 Network Load Balancing

### The Hook (Story Mode)

Imagine a single cashier at a supermarket trying to serve 200 customers alone during a holiday rush — the line would stretch out the door, and if that cashier got sick, the whole store would stop selling anything. Now imagine 10 cashiers sharing that same crowd evenly. That's load balancing: spreading work so no single point gets overwhelmed or becomes a single point of failure.

### The Explanation

**Load balancing** distributes network traffic across multiple servers or links, so no single device is overloaded. It's essential for popular websites and apps that serve millions of users simultaneously — think Instagram or a bank's online portal during peak hours.

### Benefits of Load Balancing

* Improves speed and response time for users.
* Reduces risk of total failure — if one server goes down, others keep serving requests.
* Provides a smoother, more consistent user experience.
* Helps a system handle sudden traffic spikes (like a viral post or a sale event).

### Basic Load Balancing Methods

* **Round Robin** — sends each new request to the next server in a simple rotating order (Server 1, then 2, then 3, then back to 1...).
* **Least Connection** — sends new traffic to whichever server currently has the *fewest* active connections, keeping load genuinely even.
* **IP Hash** — uses the requester's IP address to consistently route them to the *same* server each time — useful when a user's session data needs to "stick" to one server.

### The Practical Walkthrough

Let's simulate Round Robin load balancing across 3 servers with 6 incoming requests:

| Request # | Assigned Server (Round Robin) |
|---|---|
| 1 | Server A |
| 2 | Server B |
| 3 | Server C |
| 4 | Server A |
| 5 | Server B |
| 6 | Server C |

**What just happened?** Instead of Server A handling all 6 requests alone (and possibly crashing), the load balancer spread the work evenly, keeping every server comfortably busy instead of dangerously overloaded.

### Interactive Stop-Point

**Pause & Think:** A shopping website is having a massive one-day sale, and traffic is 50x higher than normal. Which load balancing method — Round Robin, Least Connection, or IP Hash — would likely handle the surge *most* fairly if some requests (like checking out with payment) take much longer to process than others (like just browsing)? Why?

### Quick Recap

Load balancing spreads network traffic across multiple servers using strategies like Round Robin, Least Connection, or IP Hash — keeping large systems fast, reliable, and resistant to single points of failure.

---

## 1.14 Network Security

### The Hook (Story Mode)

Discuss with your class: a hospital stores CT scans, prescriptions, and personal health records of every patient on its network. If that network were left unprotected, what could a hacker actually do with that data — and who would be harmed? Network security exists precisely to prevent that nightmare scenario, in hospitals, banks, schools, and your own home alike.

### The Explanation

**Network security** protects networks, devices, and data from unauthorized access, damage, or theft.

**Firewalls**

A firewall is a security device or software that controls incoming and outgoing network traffic, blocking harmful or suspicious data. Think of a firewall as a strict bouncer at a club entrance — checking everyone's ID (data) and turning away anything on the "not allowed" list.

```
  Internet (Unsafe)  --->  [ FIREWALL ]  --->  Home/Office Network (Safe)
                              |
                    Blocks harmful traffic
                    Allows legitimate traffic
```

**Encryption**

Encryption transforms readable data into a scrambled, unreadable form that only authorized parties (with the correct key) can decode. It's the backbone of secure online banking, private messaging, and HTTPS websites (as covered in 1.7).

**Access Control**

Access control decides *who* is allowed to use specific parts of a network or system. Usernames, passwords, and permission levels are the most common tools — ensuring, for example, that a regular employee can't access the company's financial records, even if they're on the same network as the finance team.

**Common Network Security Threats**

* **Viruses and malware** — malicious software that damages systems or steals data.
* **Hackers** — individuals or groups attempting to break into systems to steal information.
* **Phishing** — tricking users into voluntarily revealing sensitive information (like fake "your account is locked" emails).
* **Denial of Service (DoS) attacks** — flooding a service with fake traffic until it can no longer respond to real users.

### The Practical Walkthrough

Let's map each threat to its defense:

| Threat | Primary Defense |
|---|---|
| Malware/viruses | Antivirus software + firewall |
| Data interception on public Wi-Fi | Encryption (HTTPS, VPN) |
| Unauthorized employee snooping | Access control (permissions, roles) |
| Phishing emails | User awareness/training + email filtering |
| Denial of Service floods | Load balancing (1.13) + traffic filtering firewalls |

**What just happened?** You just built a basic security mapping — matching threats to defenses — which is the exact first step real security teams take when designing protection for any network, from a hospital to a single home router.

### Interactive Stop-Point

**Pause & Think (Hospital scenario):** How does network security specifically protect something as sensitive as a patient's CT scan? Which two defenses (firewall, encryption, access control) matter most for this specific case, and why?

### Quick Recap

Network security combines firewalls (blocking bad traffic), encryption (scrambling data), and access control (limiting who can see what) to defend against malware, hackers, phishing, and denial-of-service attacks.

---

## 1.15 Data Backup and Recovery

### The Hook (Story Mode)

Imagine spending six months writing a book on your laptop, with zero backups — and then your hard drive fails overnight. Every writer, student, and professional has heard (or lived) some version of this story. Backup exists so that "my laptop crashed" is a minor inconvenience, not a catastrophe.

### The Explanation

**Data backup** means creating a copy of important data so it can be restored if the original is lost or damaged — due to viruses, hardware failure, accidental deletion, or theft. **Recovery** is the process of actually restoring that data when disaster strikes.

### Types of Data Backups

* **Full backup** — copies *all* data at once. Simple and complete, but slow and storage-heavy if done frequently.
* **Incremental backup** — copies only the data that changed *since the last backup* (of any type). Fast and storage-efficient, but restoring requires the full backup plus every incremental backup since.
* **Differential backup** — copies all changes made *since the last full backup*. A middle ground: faster than a full backup, but simpler to restore than incremental (you only need the last full backup + the latest differential).

### Data Recovery Methods

* **Restoring from backup files** — the most reliable method, using previously saved copies.
* **Recovery software** — specialized tools that can often retrieve accidentally deleted files, even without a formal backup.
* **System restore** — rolls an operating system back to an earlier saved state.
* **Professional data recovery services** — for physically damaged drives, specialists can sometimes extract data directly from failing hardware.

### The Practical Walkthrough

Comparing backup types with a simple weekly example:

| Day | Full Backup Approach | Incremental Approach | Differential Approach |
|---|---|---|---|
| Monday | Full backup (100%) | Full backup (100%) | Full backup (100%) |
| Tuesday | Full backup again (100%) | Only Monday→Tuesday changes | All changes since Monday |
| Wednesday | Full backup again (100%) | Only Tuesday→Wednesday changes | All changes since Monday |
| Restore needed on Thursday | Use Wednesday's full copy | Need Monday + Tue + Wed increments, in order | Need Monday's full + Wednesday's differential only |

**What just happened?** You can now see the real trade-off: incremental backups save the most storage space day-to-day, but full recovery takes longer because you need every piece in the correct order; differential backups strike a practical balance most organizations actually prefer.

### Interactive Stop-Point

**Pause & Think:** Your school wants to back up all student records every night, but storage space is limited and the IT team has a small budget. Would you recommend full, incremental, or differential backups — and what would you tell them about the trade-off they're accepting?

### Quick Recap

Regular backups (full, incremental, or differential) protect against data loss, and having a clear recovery method ready turns a potential disaster into a routine fix.

---

## 1.16 Usability and Security Tradeoffs

### The Hook (Story Mode)

A company mandates a password policy: 16 characters, must include symbols, numbers, uppercase and lowercase letters, and must be changed every 30 days. Within a month, half the office has a sticky note on their monitor with their password written in plain sight. The security team made the *system* harder to break into — but accidentally made the *humans* using it the weakest link. This is the eternal tug-of-war between usability and security.

### The Explanation

**Usability** means how easy a system is to learn and use — clear, quick, and low-friction. **Security** means protecting a system from unauthorized access, viruses, and hackers.

The uncomfortable truth: **these two goals often pull in opposite directions.**

* Strong, complex passwords are harder to remember.
* Extra login steps (like two-factor authentication) slow users down, even though they add real protection.
* Fewer restrictions make a system pleasant and fast to use — but also easier to break into.
* Removing all security friction increases convenience *and* risk, simultaneously.

The goal is never "maximum security" or "maximum usability" alone — it's finding the right **balance** for the specific system and its users.

### The Practical Walkthrough

Let's compare real trade-off decisions side by side:

| Design Choice | Usability Impact | Security Impact |
|---|---|---|
| No password required | Excellent — instant access | Terrible — anyone can get in |
| Simple 4-digit PIN | Good — quick and memorable | Weak — easy to guess or brute-force |
| Strong password + 2FA | Slower — extra steps each login | Strong — much harder to breach |
| Password expires every 30 days | Poor — hard to remember new passwords constantly | Mixed — can actually *backfire* if it causes weak, predictable password patterns (like `Password1`, `Password2`...) |
| Biometric login (fingerprint/face) | Excellent — fast and natural | Strong, but raises different privacy questions |

**What just happened?** You just walked through the exact kind of trade-off analysis real security teams debate constantly — there is rarely a "perfect" answer, only an appropriate balance for a given system's users and the value of what it's protecting.

### Interactive Stop-Point

**Pause & Think:** Why does forcing employees to use extremely complex, frequently-changing passwords often backfire and make a company *less* secure overall, rather than more? What would you propose instead that keeps strong security *without* pushing people toward sticky notes?

### Quick Recap

Usability and security constantly trade off against each other — good system design doesn't chase either extreme, but finds a balance appropriate to what's being protected and who's using it.

---

## Chapter Summary

| Concept | Definition |
|---|---|
| **Computer Network** | A group of connected computers and devices that share data, resources, and services. |
| **Network Architecture** | The design and organization of a network — how devices connect and how communication happens. |
| **Network Topology** | The layout/arrangement of devices and connections — star, bus, ring, mesh, or tree. |
| **LAN** | A network connecting devices within a small area, like a home, school, or office. |
| **WAN** | A network connecting devices/networks over large geographical areas — cities, countries, continents. |
| **Internet** | The largest public network, connecting millions of devices and networks worldwide. |
| **Networking Devices** | Hardware like switches, routers, modems, NICs, and access points that connect devices and manage communication. |
| **OSI Model** | A 7-layer model explaining how data travels from one device to another across a network. |
| **Network Protocol** | A set of rules controlling how data is sent, received, and understood between devices. |
| **IP Address** | A unique address assigned to a device so it can be identified on a network. |
| **Subnetting** | Dividing a large network into smaller networks for better management and security. |
| **Network Security** | Methods used to protect networks, devices, and data from unauthorized access, misuse, or attack. |

---

## End-of-Chapter Exercise

### Multiple Choice Questions

1. A computer network is:
   (a) A single computer system (b) A group of connected computers and devices (c) A software program (d) A storage device

2. The device used to connect a computer to a network is:
   (a) Monitor (b) Keyboard (c) Network Interface Card (NIC) (d) Printer

3. A network that covers a small geographical area, such as a school or office, is:
   (a) WAN (b) MAN (c) LAN (d) Internet

4. The topology that uses a central hub or switch is:
   (a) Bus Topology (b) Ring Topology (c) Star Topology (d) Mesh Topology

5. The OSI model contains:
   (a) Five layers (b) Six layers (c) Seven layers (d) Eight layers

6. The protocol mainly used to view web pages is:
   (a) FTP (b) DNS (c) TCP (d) HTTP

7. The main function of a router is to:
   (a) Store data (b) Connect devices within a network (c) Connect different networks (d) Display web pages

8. DNS is used to:
   (a) Transfer files (b) Protect data (c) Convert domain names into IP addresses (d) Connect hardware devices

9. The device that converts digital signals for Internet transmission is:
   (a) Switch (b) Hub (c) Modem (d) NIC

10. The topology that provides the highest reliability is:
    (a) Bus topology (b) Ring topology (c) Star topology (d) Mesh topology

**Answer Key:** 1-b, 2-c, 3-c, 4-c, 5-c, 6-d, 7-c, 8-c, 9-c, 10-d

### Short Questions

1. What is a computer network?
2. Write two uses of computer networks.
3. What is network architecture?
4. Name any two components of a computer network.
5. What is the OSI model?
6. Write the names of any two network topologies.
7. What is a Local Area Network (LAN)?
8. What is the function of a router?
9. What is a network protocol?
10. What is the purpose of DNS?

### Long Questions

1. Define a computer network. Explain its importance and uses in daily life.
2. Explain network architecture and describe the main components of a computer network.
3. What is the OSI model? Explain its layers and their functions.
4. Define network topology. Explain bus, star, ring, and mesh topologies with advantages and disadvantages.
5. Explain the types of computer networks. Describe LAN, WAN, and the Internet.
6. Describe the main networking devices used in a computer network and explain their functions.
7. What are network protocols? Explain TCP/IP, HTTP, FTP, and DNS.
8. Explain IP addressing. Describe IPv4, IPv6, the default gateway, and subnetting.
9. Explain the trade-off between usability and security, with real-world examples.
10. Describe the different types of data backup and recovery methods, and explain when each is most appropriate.

---

*End of Chapter 1: Computer Networks.*
