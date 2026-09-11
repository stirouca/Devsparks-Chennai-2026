# Hands-on Lab: Building a Modern To-Do Application with IBM Bob

In this hands-on lab, you will learn how to use **IBM Bob** as an AI-powered development assistant to design, generate, troubleshoot, and enhance a modern web-based To-Do application.

Using natural language prompts, you will interact with Bob to create a complete full-stack application consisting of:

- A **Python Flask** backend
- An **HTML, CSS, and JavaScript** frontend
- An **in-memory database** for storing tasks
- A modern and responsive user interface

Throughout the lab, you will explore how Bob can assist with application planning, code generation, debugging, and UI enhancement, significantly accelerating the software development lifecycle.

#### Tech Stack

![Open Folder](images-lab1/img11.png)

#### TODO App

![Enhanced Application UI](images-lab1/img10.png)

---

# 1. Lab Details

<details><summary>Click for more info</summary>

## Lab Objectives

<details><summary>Click for more info</summary>

By the end of this lab, you will be able to:

- Understand the IBM Bob development workflow
- Use Bob's **Plan Mode** to generate an implementation plan
- Use Bob's **Agent Mode** to generate application code
- Build a full-stack To-Do application using AI-assisted development
- Resolve common development issues using Bob
- Enhance the application's user experience through conversational prompts
- Run and test a Flask-based web application

</details>

## Prerequisites

<details><summary>Click for more info</summary>

Before starting the lab, ensure you have the following:

#### Software Requirements

- IBM Bob IDE
- Python 3.x installed

#### Knowledge Requirements

Basic understanding of:

- Python programming
- Web applications
- REST APIs
- HTML, CSS, and JavaScript

</details>

## Solution Architecture

<details><summary>Click for more info</summary>


The application created in this lab uses the following architecture:

#### Frontend

- HTML
- CSS
- JavaScript

#### Backend

- Python
- Flask Framework

#### Data Storage

- In-memory database

#### Communication

- REST APIs using JavaScript Fetch API
</details>
</details>

---

# 2. Lab Tasks

## Task 1: IBM Bob Installation and Onboarding

<details><summary>Click for more info</summary>


1. Install Bob IDE using the [link](./bob-install.md#user-content-1-install-the-ibm-bob-ide). 

2. Register for the IBM Bob Trial license using the [link](./bob-install.md#user-content-2-register-for-an-ibm-bob-trial-licence).

3. Login to the BOB using the [link](./bob-install.md#user-content-3-sign-in-to-the-ibm-bob-ide-using-the-trial-licence). 

</details>

---

## Task 2: Open a Workspace in IBM Bob

<details><summary>Click for more info</summary>


### Step 1: Launch IBM Bob IDE

Open the IBM Bob IDE.

### Step 2: Open a Workspace Folder

Click **Open Folder**.

![Open Folder](images-lab1/img12.png)

Select a new folder that will be used as your application workspace.

![Choose Workspace Folder](images-lab1/img13.png)

The workspace is now opened.

### Step 3: Trust the Workspace

To allow Bob to perform development activities, the workspace must be trusted.

Click **Restricted Mode**.

![Restricted Mode](images-lab1/img14.png)

Select **Trust**.

![Trust Workspace](images-lab1/img15.png)

### Step 4: Switch to Plan Mode

Choose **Plan Mode**.

![Plan Mode](images-lab1/img16.png)

</details>

---

## Task 3: Generate the Application Plan

<details><summary>Click for more info</summary>

In this task, Bob helps define the application's architecture and implementation strategy before code generation begins.

### Step 1: Provide the Initial Prompt

Enter the following prompt in the chat window:

```text
I want to create a simple To-Do application with Python/Flask backend, HTML/CSS/JavaScript frontend, and an in-memory database for data storage.

The user interface should have a modern, responsive, and visually appealing look and feel.

Please help me with the implementation plan.
```

In case, if you are not familar with python you can simply change `Python/Flask` with `Java 17/springboot` in the prompt to create java based application.


![Initial Prompt](images-lab1/img17.png)

### Step 2: Define Application Features

Bob may ask additional questions to better understand your requirements.

Example:

> What To-Do features should the application support?

Choose an option similar to:

> Full-featured - All of the above plus task priorities and due dates

![Select Features](images-lab1/img18.png)

### Step 3: Define Frontend Communication

Bob may ask:

> How should the frontend communicate with the Flask backend?

Select an option similar to:

> REST API - JavaScript fetch calls to Flask JSON endpoints (no page reloads)

![Select REST API](images-lab1/img19.png)

### Step 4: Define Visual Style

Bob may ask:

> What visual style should the UI follow?

Choose an option similar to:

> Minimal & Clean - White/light grey background, subtle shadows, system fonts

![Select Visual Style](images-lab1/img20.png)

</details>

---

## Task 4: Review and Approve the Plan

<details><summary>Click for more info</summary>

### Step 1: Review Plan Generation

Bob may request approval to create planning artefacts.

Click **Approve Once**.

![Approve Plan Creation](images-lab1/img21.png)

### Step 2: Validate and Proceed

Review the generated plan.

If satisfied, enter:

```text
OK Proceed
```

![Proceed with Plan](images-lab1/img22.png)

### Step 3: Switch to Agent Mode

Bob may request approval to move from **Plan Mode** to **Agent Mode** for code generation.

Click **Approve Once**.

![Approve Agent Mode](images-lab1/img23.png)

### Step 4: Approve Generated Tasks

Bob may display a task list representing the work required to build the application.

Approve the request.

![Approve Task List](images-lab1/img24.png)

### Step 5: Continue Approvals

Bob may require additional approvals while generating source code and project files.

![Additional Approval](images-lab1/img25.png)

![Additional Approval](images-lab1/img26.png)

Once complete, Bob creates the application source code and project structure.

![Generated Project Files](images-lab1/img27.png)

</details>


---

## Task 5: Run the Application


<details><summary>Click for more info</summary>


### Step 1: Request Runtime Instructions

Ask Bob to generate the commands required to create and configure a virtual environment.

Prompt:

```text
To run the application, can you provide the commands to create a Python virtual environment and start the application?
```

![Request Runtime Instructions](images-lab1/img28.png)

Bob generates the required commands.

![Generated Runtime Commands](images-lab1/img29.png)

### Step 2: Execute the Commands

Run the generated commands in the integrated terminal.

![Run Command 1](images-lab1/img30.png)

![Run Command 2](images-lab1/img31.png)

![Run Command 3](images-lab1/img32.png)

### Step 3: Launch the Application

Open the application URL in your browser:

```text
http://127.0.0.1:5000
```

![Launch Application](images-lab1/img33.png)

The application is displayed.
</details>


---

## Task 6: Troubleshoot Application Issues Using Bob

<details><summary>Click for more info</summary>

AI-assisted troubleshooting is one of the most valuable capabilities of IBM Bob.

### Scenario 1: Add Task Button Not Working

Suppose the **Add Task** button is not functioning.

Ask Bob:

```text
Add Task button is not working
```

![Report Add Task Issue](images-lab1/img34.png)

Bob analyses the issue and identifies a CORS-related problem.

![CORS Fix](images-lab1/img35.png)

### Scenario 2: Issue Persists

If the issue still exists, provide more context:

```text
Still it is not working. I am using http://127.0.0.1:5000/
```

![Provide Additional Context](images-lab1/img36.png)

Bob identifies and corrects the URL configuration issue.

![URL Configuration Fix](images-lab1/img37.png)

The application should now function correctly.

### Verify Application Functionality

Add a few sample tasks to validate the solution.

![Verify Application](images-lab1/img38.png)

</details>

---

## Task 7: Enhance the User Interface

<details><summary>Click for more info</summary>

The initial version of the application is functional but may have a basic appearance.

### Step 1: Request UI Improvements

Ask Bob to modernise the application layout.

Prompt:

```text
Can you create a home page with a header, title, and left navigation menu?
```

![Request UI Improvements](images-lab1/img39.png)

Bob updates the frontend code and generates an improved interface.

![Updated Frontend Code](images-lab1/img40.png)

### Step 2: Refresh the Application

Refresh the browser to view the updated design.

![Enhanced Application UI](images-lab1/img41.png)

The application now includes:

- Header section
- Navigation menu
- Improved layout
- Better user experience
- More professional appearance

</details>

---



# 3. Key Takeaways

<details><summary>Click for more info</summary>

During this lab, IBM Bob assisted in:

- Generating an architectural plan
- Creating project files and source code
- Implementing a Flask backend
- Building a JavaScript frontend
- Creating REST APIs
- Troubleshooting application issues
- Resolving CORS and configuration problems
- Enhancing the user interface
- Accelerating end-to-end application development

### Conclusion

In this lab, you successfully used **IBM Bob** to create a modern full-stack To-Do application through natural language interactions. Instead of manually designing, coding, troubleshooting, and enhancing the entire solution, Bob acted as an AI development assistant throughout the process.

This exercise demonstrated how IBM Bob can significantly improve developer productivity by helping with planning, code generation, debugging, and UI improvements, enabling teams to build and modernise applications faster while maintaining development quality and consistency.

</details>