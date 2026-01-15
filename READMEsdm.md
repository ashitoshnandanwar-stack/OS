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

<hr>

## Testing

### 🔹 Introduction to Software Testing
- Software Testing is the process of evaluating a software application to ensure that it:Works as expected
```
Meets user requirements
Is free from defects
It helps in identifying errors, missing requirements, and gaps between expected and actual results.

In simple words:
Testing checks whether the software is correct, complete, and reliable.
```
🔹 Why Testing Code is Important
```
Finds bugs before users do
Improves software quality
Saves cost (fixing bugs later is expensive)
Ensures customer satisfaction
Increases reliability and security
Confirms that requirements are met
Reduces risk of failure in production
```

🔹 Verification and Validation
| Aspect   | Verification                         | Validation                           |
| -------- | ------------------------------------ | ------------------------------------ |
| Meaning  | “Are we building the product right?” | “Are we building the right product?” |
| Focus    | Process & documents                  | Final product                        |
| Type     | Static (no execution)                | Dynamic (with execution)             |
| Examples | Reviews, inspections, walkthroughs   | Testing, user acceptance             |
| Stage    | During development                   | After development                    |

🔹 Quality Assurance vs Quality Control vs Testing
| Term                       | Meaning                        | Focus            |
| -------------------------- | ------------------------------ | ---------------- |
| **Quality Assurance (QA)** | Prevents defects               | Process-oriented |
| **Quality Control (QC)**   | Finds defects                  | Product-oriented |
| **Testing**                | Executes software to find bugs | Product behavior |

```
QA: Define standards, process, methodology
QC: Inspect and review the product
Testing: Run the software to detect errors

Example:
QA → “Follow coding standards”
QC → “Review code”
Testing → “Run application and check output”
```
🔹 Principles of Software Testing
```
1.Testing shows presence of defects
  It proves bugs exist, not their absence.

2.Exhaustive testing is impossible
  You can’t test everything; prioritize.

3.Early testing saves time and cost
  Find defects in early stages.

4.Defect clustering
  A small number of modules usually contain most of the defects.
  In real projects, you will often find that 80% of the bugs are found in 20% of the modules.
  These parts of the system are called defect-prone areas.

5.Pesticide paradox
 If the same set of test cases is repeated again and again, they will eventually stop finding new bugs.
 Just like insects become resistant to the same pesticide over time, software becomes “immune” to the same tests.
 Existing test cases   may pass, but new defects can still exist.

6.Testing is context dependent
  Different apps need different testing.

7.Absence of errors is a fallacy
  Bug-free software may still fail if it doesn’t meet user needs.

These concepts form the foundation of Software Testing.
```

### 🔹 Introduction to STLC (Software Testing Life Cycle)

<img width="565" height="468" alt="image" src="https://github.com/user-attachments/assets/08e701a8-b108-4600-829b-1ed80693a0b7" />

Phases of STLC:
```
Requirement Analysis – Understand what to test
Test Planning – Strategy, tools, effort, schedule
Test Case Design – Write test cases & test data
Test Environment Setup – Prepare hardware/software
Test Execution – Run test cases, log defects
Test Cycle Closure – Report, evaluate, improve
```

#### 🔹 V-Model (Verification & Validation Model)

<img width="644" height="459" alt="image" src="https://github.com/user-attachments/assets/fc9fd241-e5bd-4548-801f-032c77ef1826" />

- The V-Model shows the relation between development phases and testing phase
- Left side: Verification (planning & designing)
- Right side: Validation (testing & execution)
- Each development stage has a corresponding testing stage.

#### 🔹 Types of Testing
1️⃣ Manual Testing
```
Testing done by human without tools
Example: Checking login form manually
Best for: UI, exploratory testing
```

2️⃣ Automation Testing
```
Testing using scripts & tools
Example: Selenium script for login
Best for: Repetitive, regression testing
```

| Manual             | Automation          |
| ------------------ | ------------------- |
| Slow               | Fast                |
| Human effort       | Tool based          |
| Low cost initially | High setup cost     |
| Good for UI        | Good for regression |

🔹 Tools Used for Automation Testing
```
Selenium – Web automation
Cypress – Modern web testing
TestNG / JUnit – Test frameworks
Appium – Mobile app testing
Postman – API testing
JMeter – Performance testing
UFT (QTP) – Commercial tool
```

#### 🔹 Testing Methods

| Type                  | Knowledge of Code                   | Focus                                         | Example                                      |
| --------------------- | ----------------------------------- | --------------------------------------------- | -------------------------------------------- |
| **White Box Testing** | Full access to source code          | Internal logic, paths, conditions, loops      | Unit testing by a developer                  |
| **Black Box Testing** | No knowledge of code                | Functionality as per requirements             | Testing login page with valid/invalid inputs |
| **Grey Box Testing**  | Partial knowledge of code/structure | Combination of internal logic + functionality | Testing APIs with knowledge of DB schema     |

Examples:
```
White-box → Unit testing by developer
Black-box → Functional testing by tester
Grey-box → Security & integration testing
```

🔹 Functional Testing (Concept)
- Checks what the system does.
```
Includes:
Unit Testing
Integration Testing
System Testing
Acceptance Testing
Smoke Testing
Sanity Testing
Regression Testing

Example:
Login works
Payment is successful
Report is generated
```
🔹 Non-Functional Testing (Concept)
- Checks how the system performs.
```
Includes:
Performance Testing
Load Testing
Stress Testing
Security Testing
Usability Testing
Compatibility Testing
Scalability Testing

Example:
Page loads in 2 seconds
App works on Chrome & Firefox
System handles 1000 users
```

- Together, STLC + V-Model + Testing Types build a strong foundation for software testing concepts.

Example:
```
Consider a real-time example of an Online Shopping (E-commerce) Website like Amazon or Flipkart.

🔹 Functional Testing (What the system does)
Functional testing checks whether features work as per requirements.
Real-time examples:
Verify user can register with valid details
Check login with correct and incorrect credentials
Add product to cart
Apply coupon code and verify discount
Place an order successfully
Verify payment using UPI/Card
Check order confirmation email/SMS
👉 These tests validate functions and business logic.

🔹 Non-Functional Testing (How well the system performs)
Non-functional testing checks performance, usability, security, etc.
Real-time examples:
Page should load within 3 seconds (Performance testing)
Website should handle 10,000 users at a time (Load testing)
App should not crash on low network (Reliability testing)
Password must be encrypted (Security testing)
UI should be easy to use on mobile & desktop (Usability testing)
System should recover after server failure (Recovery testing)
👉 These tests validate quality attributes of the system.

In short:
Functional Testing → “Is the feature working?”
Non-Functional Testing → “How well is it working?”
```

<hr>

## Selenium

### 🔹 Introduction to Selenium (Using Eclipse IDE)
- Selenium is an open-source automation tool used to test web applications.
- It supports multiple browsers (Chrome, Firefox, Edge) and languages (Java, Python, C#).
- Using Eclipse IDE + Java + Selenium WebDriver is the most common setup.

### 🔹 1. Load WebDriver (Basic Setup in Java)
```
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class FirstTest {
    public static void main(String[] args) {

        System.setProperty("webdriver.chrome.driver",
                "D:\\drivers\\chromedriver.exe");

        WebDriver driver = new ChromeDriver();
        driver.get("https://example.com");
        driver.manage().window().maximize();
    }
}
```
System.setProperty(...)  →  tells where the driver file is
new ChromeDriver()  →  loads the WebDriver and opens Chrome
driver.get(url)  →  loads the web page

### 🔹 2. Selenium Commands – Locators
- Selenium finds elements using locators:
```
// By ID
driver.findElement(By.id("username"));

// By Name
driver.findElement(By.name("email"));

// By Class Name
driver.findElement(By.className("btn-login"));

// By Tag Name
driver.findElement(By.tagName("input"));

// By XPath
driver.findElement(By.xpath("//input[@type='password']"));
```

### 🔹 3. Add Interactions
✏️ Text Box
```
driver.findElement(By.id("username")).sendKeys("admin");
driver.findElement(By.id("password")).sendKeys("12345");
```

🔘 Radio Button
```
driver.findElement(By.id("male")).click();
```

☑️ Check Box
```
driver.findElement(By.id("terms")).click();
```

🔽 Drop-down Selection
```
Select s = new Select(driver.findElement(By.id("country")));
s.selectByVisibleText("India");
```

⌨️ Keyboard Actions
```
Actions act = new Actions(driver);
act.sendKeys(Keys.TAB).sendKeys("Hello").perform();
```

🖱️ Mouse Actions
```
WebElement menu = driver.findElement(By.id("menu"));
Actions act = new Actions(driver);
act.moveToElement(menu).perform();   // Hover
```

🔢 Multi-Select Drop-down
```
Select s = new Select(driver.findElement(By.id("skills")));
s.selectByVisibleText("Java");
s.selectByVisibleText("Python");
```

<hr>

## 🔹 Introduction to Delivery Pipeline
- A Delivery Pipeline is an automated flow that takes code from commit to production.
- Typical stages:  Code Commit → Build → Test → Package → Deploy → Release
- It ensures: <br>
Fast delivery <br>
Fewer errors <br>
Continuous feedback <br>
Automation of manual work <br>

- This concept is part of CI/CD (Continuous Integration & Continuous Delivery).

### 🔹 Introduction to Jenkins
- Jenkins is an open-source automation server used for:
```
Building code
Running tests
Creating artifacts
Deploying applications
Managing CI/CD pipelines

It integrates with:
Git/GitHub
Maven/Gradle
Docker
Selenium
Kubernetes
```
- an artifact is a file that is generated during a build and saved so it can be used later.

### 🔹 Jenkins Management
- From Manage Jenkins you can:
```
Install/Update plugins
Configure system settings
Manage users & security
Configure tools (JDK, Maven, Git)
Add nodes (agents/slaves)
Backup & restore Jenkins

Important sections:
Manage Plugins
Configure System
Global Tool Configuration
Nodes and Clouds
```

### 🔹 Adding Slave (Agent) Node to Jenkins
- Purpose: Distribute workload across multiple machines.

- Steps: Go to Manage Jenkins → Nodes and Clouds → New Node
```
Enter: Node name

Type: Permanent Agent

Configure: Remote root directory

Labels Launch method (SSH / JNLP)

Save and connect the node

Now Jenkins can run jobs on this slave/agent machine.
```

### 🔹 Building a Delivery Pipeline in Jenkins
Using Jenkinsfile (Pipeline as Code):
```
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Package') {
            steps {
                echo 'Creating artifact...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}

This creates a visual pipeline in Jenkins:
Build → Test → Package → Deploy
```

### 🔹 Selenium Integration with Jenkins

Purpose: Run automated Selenium tests automatically after every build.

Steps:
```
1.Install plugins:
Git
Maven
Selenium / TestNG plugins

2.Create Jenkins Job:
Choose Freestyle or Pipeline
Connect Git repository

3.Add Build Step:
mvn clean test

4.Configure Test Reports:
Post-build action → Publish TestNG / JUnit Reports

Now the flow becomes:
Code Commit → Jenkins Build → Run Selenium Tests → Generate Report → Notify Team

If Selenium tests fail:
Jenkins marks the build as FAILED

Developer is notified
```
This completes a CI/CD Delivery Pipeline with Selenium + Jenkins.

<hr>
