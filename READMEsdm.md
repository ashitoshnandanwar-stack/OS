# OS

Operating System

## Git and Github

- Git is a software and Github is a service.
- Git is a version control system. It is : popular, free & Open source, fast & scalable.
- Github - It is website that allows developers to store and manage their code using Git.
- Clone = cloining a repository on our local machine -- git clone <-some link ->
- Status = displays the state of the code -- git status
- cd = change directory
- Untracked = new file that git doesn't yet track
- modified = changed in file
- staged - file is ready to be continued
- unmodified - unchanged
- add -> commit
- add - adds new or changed files in your working directory to the Git staging area.
  git add <-flle name ->
  git add . = commit all
- commit - it is record of change
  git commit -m "some message"
- push - upload local repo content to remote repo
  git push origin main

### Software development
- Software Engineering is a systematic approach to analyze, design, develop, test, and maintain high-quality software using defined processes and models.
1. Software development lifecycle (SDLC)
   https://upload.wikimedia.org/wikipedia/commons/1/19/SDLC_-_Software_Development_Life_Cycle.jpg
   SDLC Phases
  1. Requirement Analysis
  2. Design
  3. Implementation (coding)
  4. Testing
  5. Deployment
  6. Maintainence

| Feature     | Function-Oriented | Object-Oriented |
| ----------- | ----------------- | --------------- |
| Focus       | Functions         | Objects         |
| Data        | Separate          | Encapsulated    |
| Reusability | Low               | High            |
| Examples    | C                 | Java, C++       |

- Modularity = dividing system into modules
- Cohesion = How closely related elements in a module (High cohesion = good)
- Coupling = Dependency between modules (Low coupling = good)
- Layering = Organizing system into layers (UI, Service, Database)
### 🔹 Requirements Engineering
- Requirements Engineering (RE) is the systematic process of <br>
gathering, analyzing, documenting, validating, and managing the requirements of a software system.


🔹 Types of Requirements
```
1. Functional Requirements
What the system should do
Example:
“User can login”
“System generates report”

2. Non-Functional Requirements
How the system performs
Example:
Performance (response < 2 sec)
Security (data encryption)
Reliability, Usability, Scalability

User Requirements
Written in simple language for end users
Example:
“Customer should be able to book ticket online”

System Requirements
Detailed technical description
Example:
“System shall authenticate using OTP”

Business Requirements
High-level organizational goals
Example:
“Increase online sales by 30%”
```
🔹 Steps Involved in Requirements Engineering
```
- Feasibility Study
Technical, Economic, Operational feasibility

- Requirements Elicitation
Collect requirements from stakeholders
Methods: Interview, Questionnaire, Observation, Workshop

- Requirements Analysis
Remove ambiguity and conflicts
Prioritize and refine requirements

- Requirements Specification (SRS)
Document requirements in SRS format

- Requirements Validation
Check correctness, completeness, consistency

- Requirements Management
Handle changes and updates
```
🔹 Requirement Analysis Modelling
- Requirement Analysis Modeling converts raw requirements into structured models for better understanding.
Common Models:
```
Use Case Diagram
Shows interaction between user and system
Example: Login, Register, Purchase

Data Flow Diagram (DFD)
Shows flow of data in the system
Levels: Context, Level-0, Level-1

Entity Relationship Diagram (ERD)
Shows database structure (entities & relations)
Class Diagram
Used in OO systems
Shows classes, attributes, methods

State Diagram
Shows states of an object (e.g., Order: New → Paid → Shipped)
These models help in:
Reducing ambiguity
Visualizing system behavior
Improving communication between stakeholders and developers
```

### 🔹 Characteristics of a Good Design

A good software design should have the following qualities:
```
Correctness – Fulfills all user requirements
Simplicity – Easy to understand and implement
Modularity – Divided into small, independent modules
Reusability – Components can be reused in other systems
Maintainability – Easy to modify and fix
Scalability – Can grow with new features/users
Efficiency – Uses resources (time, memory) effectively
Flexibility – Easy to adapt to changes
Low Coupling – Modules are loosely connected
High Cohesion – Each module has a single, clear purpose
```
🔹 Function Oriented vs Object Oriented System
| Aspect             | Function Oriented System | Object Oriented System           |
| ------------------ | ------------------------ | -------------------------------- |
| Focus              | Functions / Procedures   | Objects (Data + Methods)         |
| Design Approach    | Top-down                 | Bottom-up                        |
| Data Handling      | Data is global or passed | Data is encapsulated             |
| Security           | Less secure              | More secure (Encapsulation)      |
| Reusability        | Limited                  | High (Inheritance, Polymorphism) |
| Maintenance        | Difficult                | Easy                             |
| Examples           | C, Pascal                | Java, C++, C#, Python            |
| Real-world Mapping | Poor                     | Excellent (real-world modeling)  |

### Software Process Models
- A Software Process Model defines the order (sequence) of activities involved in software development such as requirement analysis, design, coding, testing, and maintenance.
- Types of process models
  1. Waterfall model <br>
     A linear and sequential model where each phase must be completed before moving to the next.<br>
     Phases = Requirement → Design → Implementation → Testing → Deployment → Maintenance <br>
     Advantages = Simple and easy to understand, Well-defined stages, Good for small projects <br>
     Disadvantages = No flexibility, Difficult to change requirements, Late testing <br>
     Best suited for : Small projects with fixed requirements <br> 
  2. Incremental model <br>
     Software is developed and delivered in small increments (parts).
  3. Iterative Model <br>
     Development starts with a simple version and improves through repeated cycles (iterations).
  4. Sprial Model <br>
     A risk-driven model combining waterfall and iterative approaches. <br>
     key features : risk analysis in every loop <br>
  5. Agile Model <br>
     A flexible and iterative model focusing on customer collaboration and rapid delivery. <br>
     Agile divides work into sprints<br>
     Key Principles : Customer involvement, Small iterations (sprints), Working software over documentation. <br>
     Projects with frequently changing requirements. <br>
     Agile development gives importance to working software.

| Model       | Key Feature            | Best For              |
| ----------- | ---------------------- | --------------------- |
| Waterfall   | Sequential             | Fixed requirements    |
| Incremental | Part-by-part delivery  | Large systems         |
| Iterative   | Repeated cycles        | Evolving requirements |
| Spiral      | Risk analysis          | High-risk projects    |
| Agile       | Customer collaboration | Changing requirements |

##### One-Line Exam Answers<br>
- Waterfall Model: Linear sequential model
- Incremental Model: Software delivered in parts
- Iterative Model: Developed through repeated cycles
- Spiral Model: Risk-driven development model
- Agile Model: Flexible, customer-centric model

### Software Product
- A Software Product is the final outcome of the software development process. <br>
Software Product = Software + Documents + Data <br>
- Two types of software Product<br>
1. Generic <br>
2. Customized <br>

| Feature      | Generic Product | Customized Product |
| ------------ | --------------- | ------------------ |
| Users        | Many users      | Single client      |
| Requirements | General         | Client-specific    |
| Cost         | Lower per user  | Higher             |
| Flexibility  | Limited         | High               |
| Example      | Browser         | Bank software      |

### UML
- UML (Unified Modeling Language) is a standard visual modeling language used to visualize, design, document, and communicate the structure and behavior of software systems—especially object-oriented systems.
- Why UML is Used (Importance) 
Provides a common language for developers and stakeholders <br>
Helps understand system requirements clearly <br>
Reduces design errors before coding <br>
Improves documentation and maintenance <br>

<hr>
## Agile Methodology
### 🔹 Introduction to Agile Development Model
- Agile is a modern software development approach that focuses on:
```
Iterative development
Customer collaboration
Fast delivery
Adapting to change
```
- Instead of building the entire product at once, Agile develops software in small cycles (iterations/sprints) and delivers working software frequently.
- Core idea:  “Build → Test → Get Feedback → Improve” in short cycles.

### 🔹 Agile Development Components
```
Product Backlog – List of all features & requirements
Sprint – Fixed time period (1–4 weeks)
Sprint Planning – Decide what to build in sprint
Daily Stand-up – Short daily meeting
Sprint Review – Demo of completed work
Sprint Retrospective – Improvement discussion
Cross-functional Team – Dev, QA, UI, etc.
Continuous Feedback – From customer & users
```

###🔹 Benefits of Agile
```
Faster delivery
Better quality
Early error detection
Customer satisfaction
Easy to handle changes
Continuous improvement
Higher team collaboration
```

### 🔹 Tools Used for Agile Web Development
| Tool             | Purpose                   |
| ---------------- | ------------------------- |
| **Jira**         | Project & task management |
| Trello           | Simple kanban board       |
| Git / GitHub     | Version control           |
| Jenkins          | CI/CD automation          |
| Slack / MS Teams | Team communication        |
| Confluence       | Documentation             |
| Figma            | UI/UX design              |

### 🔹 Scrum and Extreme Programming (XP)
| Aspect              | Scrum                                               | Extreme Programming (XP)                                   |
| ------------------- | --------------------------------------------------- | ---------------------------------------------------------- |
| Primary focus       | **Project management framework**                    | **Engineering & coding practices**                         |
| Goal                | Manage work in iterations (sprints)                 | Improve code quality and adaptability                      |
| Iteration length    | 1–4 weeks (Sprint)                                  | 1–2 weeks (Iteration)                                      |
| Roles               | Product Owner, Scrum Master, Development Team       | Programmer, Customer, Coach, Tracker                       |
| Planning            | Sprint Planning, Daily Scrum, Review, Retrospective | Planning Game, frequent releases                           |
| Technical practices | Not prescriptive about coding                       | Strongly prescriptive                                      |
| Key practices       | Backlog, Sprints, Stand-ups                         | Pair programming, TDD, Continuous Integration, Refactoring |
| Documentation       | Minimal, as needed                                  | Very light, code is primary                                |
| Change handling     | Changes allowed between sprints                     | Changes welcomed anytime                                   |

