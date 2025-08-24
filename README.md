# CS 230 Software Design Document – The Gaming Room

## Project Overview
This repository contains the completed software design document for **The Gaming Room**, a client of Creative Technology Solutions (CTS). The Gaming Room requested that we design a scalable, secure, and distributed software application to expand their game **Draw It or Lose It** from an Android-only application into a web-based, multi-platform environment. The final design supports web browsers on Windows, macOS, Linux, and mobile devices.

---

## Reflection Questions

### 1. Briefly summarize The Gaming Room client and their software requirements.
The Gaming Room is a client that produces the game *Draw It or Lose It*. Their main requirement was to expand the game into a web-based application that could support multiple operating systems and platforms simultaneously. They also required the solution to enforce unique game and team names, use secure storage and memory management techniques, and support distributed, real-time gameplay for many concurrent users.

### 2. What did you do particularly well in developing this documentation?
I did particularly well in clearly breaking down the system architecture and explaining why the chosen operating platform (Ubuntu Server LTS) is the best option. I also provided thorough details about memory management, storage solutions, distributed systems, and security. This ensured that the client could see both the technical reasoning and the business justification for each recommendation.

### 3. What about the process of working through a design document did you find helpful when developing the code?
Working through the design document forced me to think systematically before coding. By mapping out requirements such as uniqueness checks, singleton and iterator patterns, and distributed considerations, I was able to implement cleaner, more efficient code. The design document served as a blueprint, reducing the chance of errors and making the coding process much smoother.

### 4. If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?
If I were to revise one part, I would expand the section on performance optimization. Specifically, I would add more metrics and projections for scalability under high user loads. This could include benchmarking memory usage under different garbage collectors or modeling network throughput under WebSocket load. Adding quantitative data would strengthen the design by showing not only *how* it scales but *how much* it scales.

### 5. How did you interpret the user’s needs and implement them into your software design? Why is it so important to consider the user’s needs when designing?
I translated the user’s needs into technical solutions:  
- **Unique names** were enforced via database constraints and iterator pattern checks.  
- **Multi-platform support** was achieved using a web-based architecture accessible on desktops and mobile browsers.  
- **Security needs** were implemented with TLS, OAuth 2.0/JWT, and AES-256 encryption.  

It is important to consider the user’s needs because a technically strong system that doesn’t solve the client’s actual problems is ultimately a failed product. The success of the project depends on aligning technical solutions with user expectations.

### 6. How did you approach designing software? What techniques or strategies would you use in the future to analyze and design a similar software application?
I approached software design using a combination of:  
- **Top-down analysis**: breaking down the client’s needs into categories (platform, memory, storage, security, distributed systems).  
- **Design patterns**: singleton and iterator were applied to enforce requirements.  
- **Industry best practices**: security by default, modular architecture, and containerization.  

In the future, I would continue to use design documents as a roadmap, incorporate stakeholder feedback early, and leverage iterative prototypes to validate assumptions before full implementation.

---

## Repository Contents
- `CS 230 Project Software Design Template COMPLETE [Part 3].docx` – Final design document delivered to the client  
- `README.md` – This reflection file  

---
