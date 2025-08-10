# System Design

**System Design** is the process of defining the **architecture**, **components**, **data flow**, and **interfaces** of a software system with the goal of meeting specific functional and non-functional requirements such as:

1. Scalability  
2. Reliability  
3. Availability  
4. Maintainability  
5. Performance  

> *System Design is about designing how a complete software system works from the inside out — not just writing code, but thinking deeply about how parts interact, how data flows, how users engage with the system, and how it behaves at scale.*

---

##  When to Use System Design

System design becomes essential when:

1. You're building something larger than a simple script or basic app — especially if it's user-facing or meant to scale.
2. You need to ensure the system can handle:
   - **Scalability** (millions of users or operations)
   - **Reliability** (survive failures or downtime)
   - **Performance** (fast responses under load)
   - **Security** (safe access and data protection)
3. You're designing:
   - Backend infrastructure  
   - Distributed systems  
   - Microservices architecture  
   - Cloud-based applications  
   - Data-intensive pipelines  

---

##  Types of System Design

### 1. HLD – High Level Design

**HLD** is the architectural blueprint of the entire system. It answers the **"what"** and **"how"** at a broader, system-wide level.

####  Purpose:
- Defines how components interact  
- Focuses on scalability, availability, security, and tech stack choices  
- Identifies major modules, APIs, databases, servers, etc.  

####  HLD Includes:
- System architecture diagrams (e.g. `Client ↔ Load Balancer ↔ Backend ↔ DB`)  
- Microservices/modules and their responsibilities  
- Communication patterns (REST APIs, Message Queues, etc.)  
- Tech stack selection  
- Database choices and high-level schema  
- Scalability & fault-tolerance strategies (e.g. CDN, Replication)

> *Think of HLD like city planning — roads, districts, power grids, and water lines.*

---

### 2. LLD – Low Level Design

**LLD** is the detailed internal design of each component defined in HLD. It answers the **"how exactly"** questions — like creating blueprints for individual buildings in your city.

#### Purpose:
- Describes internal logic, classes, data models, algorithms, and workflows  
- Helps developers understand exactly what needs to be built  

#### LLD Includes:
- Class diagrams  
- Object relationships  
- API contract details (endpoints, parameters, response models)  
- Database table structures  
- Function definitions or pseudocode  
- Internal business logic breakdown  

---

# A. Monolithic Architecture: 
If all the components and functionalities of a project are entangled and combined in a single codebase, then it is called a monolithic architecture.

![Monolithic Example](Images/Monolithic.png)

***Monolithic Architecture has less complexity -> Easy to understand -> Higher production***
-> Also know as Centralised system.

### Why it is good?
1. In monolithic architecture all the modules are present in a single system, so they require fewer network calls.
2. It is comparatively easy to get secured.

### Disadvantages:
1. In monolithic architecture, every module is combined in a single system, so if there is an error or bug in a single module, it can destroy the complete system.
2. In monolithic architecture, whenever a single module is updated, the whole system needs to be updated to reflect the changes to the users. All modules are present in a single system and are connected to one another, so the whole system needs to be updated.
3. If there is any change in a single module's programming language or framework, it will affect the entire system.



  
     
  
