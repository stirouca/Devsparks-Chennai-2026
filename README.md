# IBM Bob: DevSparks Chennai 2026
### Three Hands-On Labs with IBM Bob IDE

---

## Plan

| S.No	| Topic	| Link | Minutes | 
|---|---|---|---|
| 1	| Intoducing Bob and Lab |	| 5| 
| 2	| Lab 1 Walkthrough	| [Link](./lab1-guide-todo-app.md) | 5| 
| 3	| Lab 1 Execution	| [Link](./lab1-guide-todo-app.md) | 25| 
| 4	| Lab 2 Walkthrough	| [Link](./lab2-guide-java-modern.md) | 5| 
| 5	| Lab 2 Execution	| [Link](./lab2-guide-java-modern.md) | 20|

---

## Labs

### 🔬 Lab 1 — TODO App Development
Develop a simple TODO Application using IBM Bob.

📖 **[Start Lab 1 → lab1-guide.md](./lab1-guide-todo-app.md)**

#### Tech Stack 
- Backend : Python, Flask Framework
- Frontend : HTML. CSS, JavaScript
- Database : In-memory db

---

### 🔬 Lab 2 — Java Modernization
Transform a **Legacy Struts 1.3 + Java 8 + SQLite** application into a modern **Spring Boot 3.x + React 18 + PostgreSQL 15** cloud-native app — using IBM Bob.

📖 **[Start Lab 2 → lab2-guide.md](./lab2-guide-java-modern.md)**

| Layer | Before | After |
|---|---|---|
| Runtime | Java 1.8 | Java 17 |
| Back-end | Apache Struts 1.3 | Spring Boot 3.x |
| Front-end | JSP + Scriptlets | React 18 SPA |
| Database | SQLite | PostgreSQL 15 + Flyway |
| Auth | HTTP Session | JWT + BCrypt |
| Deploy | WAR / Tomcat | Docker + OpenShift |

---

### 🔄 Lab 3 — AI-Powered SDLC
Use IBM Bob as an **end-to-end AI pair programmer across the entire SDLC** — from reading GitHub issues through to a documentation-ready architecture diagram. Bob is wired to GitHub CLI, Tavily web search, and Draw.io via MCP.

📖 **[Start Lab 3 → lab3-guide-sdlc.md](./lab3-guide-sdlc.md)**

| SDLC Phase | What Bob Does | Tool Used |
|---|---|---|
| Discovery | Fetches open GitHub issues | `gh` CLI |
| Planning | Researches topic with live web search | Tavily MCP |
| Design | Generates a visual design diagram | Draw.io MCP |
| Development | Implements the feature using subagents | Agent Mode |
| Documentation | Produces a final architecture diagram | Draw.io MCP |


---

## Prerequisites
- IBM Bob IDE installed → `https://bob.ibm.com/docs/ide/getting-started/install`
- **Lab 1:** Python 3
- **Lab 2:** PlantUML Markdown Preview extension in Bob IDE
- **Lab 3:** GitHub CLI (`gh`) · Tavily API key · Node.js (for Draw.io MCP)

## References
- Bob IDE Install: https://bob.ibm.com/docs/ide/getting-started/install
- GitHub CLI: https://cli.github.com/
- Tavily: https://www.tavily.com/
