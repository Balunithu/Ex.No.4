# EXPERIMENT – 4

## GENERATE THE PROMPT AND EVALUATE IT FOR DIFFERENT PROMPT PATTERNS

### Aim

To design prompts using different prompt patterns such as **Zero-shot Prompting, Few-shot Prompting, Chain-of-Thought Prompting, Persona Pattern, Reverse Prompting, Graph Prompting, and Active Prompting**, and to compare their outputs using different AI tools and evaluate the results using an **evaluation rubric**.

### Scenario / Use Case

**Use Case:** IoT-Based Smart Manufacturing and Predictive Maintenance

The manufacturing industry wants to reduce manual monitoring and improve production efficiency using **IoT devices, embedded controllers, real-time monitoring, and predictive maintenance**.

The system collects machine data such as temperature, vibration, energy consumption, and operating status. AI can analyze this data to identify abnormal conditions, predict possible machine failures, and support preventive maintenance.

### Target Audience

Manufacturing companies in sectors such as:

* Automotive
* Electronics
* Food processing
* Industrial machinery

### Main Objectives

1. Improve production efficiency by **30%**.
2. Minimize machinery downtime using predictive maintenance.
3. Enable real-time monitoring and remote control.
4. Reduce energy consumption by optimizing manufacturing processes.
5. Detect abnormal machine conditions at an early stage.

---

# Prompt Patterns

## 1. Zero-Shot Prompting

### Definition

Zero-shot prompting asks an AI system to perform a task **without providing any examples**.

### Prompt

> **"Explain how an IoT-based predictive maintenance system can improve manufacturing efficiency. Describe how sensors collect machine data, how AI analyzes the data to predict failures, and how the system can reduce downtime and energy consumption. Give a simple example from an automobile manufacturing plant."**

### Expected Output

The AI explains the complete predictive-maintenance process without being given examples.

### Evaluation

* Relevance: High
* Simplicity: High
* Detail: Medium
* Accuracy: High

---

## 2. Few-Shot Prompting

### Definition

Few-shot prompting provides the AI with **a few examples** before asking it to perform a similar task.

### Prompt

> **"Identify the machine condition and recommended action from the given sensor information.**
>
> **Example 1:**
> Temperature = 45°C, Vibration = Low
> Condition = Normal
> Action = Continue operation
>
> **Example 2:**
> Temperature = 75°C, Vibration = High
> Condition = Abnormal
> Action = Inspect machine immediately
>
> **Example 3:**
> Temperature = 85°C, Vibration = Very High
> Condition = Critical
> Action = Stop machine and perform maintenance
>
> **Now analyze:**
> Temperature = 80°C, Vibration = High
> Identify the machine condition and recommend an appropriate action."**

### Expected Output

**Condition:** Critical/Abnormal
**Action:** Inspect the machine immediately and schedule maintenance to prevent failure.

### Evaluation

Few-shot prompting provides more consistent output because examples guide the AI's expected response format.

---

# 3. Chain-of-Thought Prompting

### Definition

Chain-of-Thought prompting asks the AI to solve a complex problem through a sequence of reasoning steps.

### Prompt

> **"Analyze the following smart manufacturing situation step by step:**
>
> A production machine normally operates at 60°C with low vibration. The IoT sensors suddenly report a temperature of 85°C and high vibration. Explain the sequence of actions that a predictive maintenance system should take, from sensor-data collection to maintenance recommendation. Identify the abnormal condition, possible causes, risk level, and recommended action."**

### Expected Output Structure

1. Collect sensor data.
2. Compare the current readings with normal operating values.
3. Detect abnormal temperature and vibration.
4. Identify possible machine problems.
5. Determine the risk level.
6. Generate a maintenance alert.
7. Recommend inspection or maintenance.
8. Record the event for future predictive analysis.

### Evaluation

Chain-of-Thought prompting is useful for **complex decision-making and multi-step engineering problems**.

---

# 4. Persona Pattern

### Definition

Persona prompting assigns a specific **role or expertise** to the AI before asking it to perform a task.

### Prompt

> **"Act as an experienced Industrial IoT Engineer and Predictive Maintenance Specialist. Design an IoT-based predictive maintenance solution for an automobile manufacturing plant. Explain the sensors required, data collection process, AI analysis, real-time monitoring, failure prediction, alerts, and expected benefits in simple technical language."**

### Expected Output

The AI responds from the perspective of an Industrial IoT and predictive-maintenance expert and provides a technically focused solution.

### Evaluation

Persona prompting helps generate **domain-specific and professional responses**.

---

# 5. Reverse Prompting

### Definition

Reverse prompting starts with a desired output or solution and asks the AI to determine the **prompt or requirements needed to generate that output**.

### Prompt

> **"I want an AI system to generate a complete proposal for an IoT-based predictive maintenance system for a manufacturing plant. The proposal must include sensors, data collection, cloud/edge processing, AI-based failure prediction, real-time dashboard, alerts, security, implementation steps, and expected benefits. Create an optimized prompt that I can give to an AI tool to generate this proposal."**

### Expected Output

The AI generates a detailed prompt containing requirements such as:

* System architecture
* Sensors
* Data processing
* AI/ML model
* Dashboard
* Alerts
* Security
* Implementation
* Benefits

### Evaluation

Reverse prompting is useful when the user knows **what output is required but does not know how to formulate the best prompt**.

---

# 6. Graph Prompting

### Definition

Graph prompting represents information using **nodes and relationships** to help the AI understand connections between different components.

### Prompt

> **"Represent an IoT-based predictive maintenance system as a graph. Use nodes for Sensors, IoT Gateway, Edge Device, Cloud Platform, AI Model, Database, Dashboard, Alert System, and Maintenance Team. Show the relationships and direction of data flow between the nodes. Then explain how the graph supports predictive maintenance."**

### Expected Graph

```text
[Machine]
    |
    ↓
[IoT Sensors]
    |
    ↓
[IoT Gateway]
    |
    ↓
[Edge Device]
    |
    ↓
[Cloud Platform]
    |
    ↓
[AI Predictive Model]
    |
    ↓
[Database] ←→ [Dashboard]
    |
    ↓
[Alert System]
    |
    ↓
[Maintenance Team]
```

### Evaluation

Graph prompting is useful for understanding **system architecture, relationships, dependencies, and data flow**.

---

# 7. Active Prompting

### Definition

Active prompting allows the AI to **ask for important information or clarification** before generating the final solution.

### Prompt

> **"You are designing an IoT-based predictive maintenance system for a manufacturing plant. Before proposing the final solution, identify the most important missing information you need from the manufacturing team. Ask questions about machine types, sensor availability, operating conditions, historical maintenance data, network connectivity, production requirements, and acceptable downtime. After receiving the answers, generate the predictive maintenance solution."**

### Expected Output

The AI may ask:

1. What types of machines are being monitored?
2. What sensors are currently available?
3. Is historical machine-failure data available?
4. What network connectivity is available?
5. How frequently should sensor data be collected?
6. What level of downtime is acceptable?
7. Is cloud or edge processing preferred?

### Evaluation

Active prompting is useful when **important requirements are unknown** and additional information is needed before designing the solution.

---

# Evaluation Using Rubrics

Each prompt can be evaluated using the following criteria.

| Criteria             |  Weight |
| -------------------- | ------: |
| Relevance            |      20 |
| Accuracy             |      20 |
| Completeness         |      20 |
| Clarity              |      15 |
| Technical Detail     |      15 |
| Practical Usefulness |      10 |
| **Total**            | **100** |

### Sample Evaluation

| Prompt Pattern   | Relevance | Accuracy | Completeness | Clarity | Technical Detail | Usefulness |    Total |
| ---------------- | --------: | -------: | -----------: | ------: | ---------------: | ---------: | -------: |
| Zero-Shot        |        18 |       18 |           15 |      19 |               14 |          9 |   **93** |
| Few-Shot         |        19 |       19 |           17 |      19 |               15 |         10 |   **99** |
| Chain-of-Thought |        19 |       18 |           19 |      17 |               19 |         10 | **102*** |
| Persona          |        19 |       19 |           18 |      18 |               19 |         10 | **103*** |
| Reverse          |        18 |       18 |           18 |      17 |               18 |         10 |   **99** |
| Graph            |        19 |       19 |           19 |      18 |               19 |         10 | **104*** |
| Active           |        19 |       19 |           19 |      18 |               18 |         10 | **103*** |

**Note:** To keep the score within 100, each criterion should be normalized according to its stated weight. The table above is illustrative; actual scores should be entered after testing the prompts in the selected AI tools.

### Recommended Rubric Scoring

Use:

* **5 – Excellent**
* **4 – Very Good**
* **3 – Good**
* **2 – Fair**
* **1 – Poor**

Then calculate:

**Score = (Obtained Score / Maximum Score) × 100**

---

# Comparison of Prompt Patterns

| Prompt Pattern    | Main Purpose                 | Best Used For                            |
| ----------------- | ---------------------------- | ---------------------------------------- |
| Zero-Shot         | Direct instruction           | General explanations                     |
| Few-Shot          | Gives examples               | Classification and consistent formatting |
| Chain-of-Thought  | Multi-step reasoning         | Complex engineering problems             |
| Persona           | Assigns expertise            | Domain-specific responses                |
| Reverse Prompting | Creates an effective prompt  | Prompt optimization                      |
| Graph Prompting   | Shows relationships          | Architecture and data flow               |
| Active Prompting  | Collects missing information | Requirement gathering                    |

---

# Procedure

1. Define the **IoT-based smart manufacturing** scenario.
2. Identify the objectives and target audience.
3. Select the seven prompt patterns.
4. Design a suitable prompt for each pattern.
5. Execute the prompts using selected AI tools.
6. Record the generated responses.
7. Compare the responses based on relevance, accuracy, completeness, clarity, technical detail, and usefulness.
8. Apply the rubric-based evaluation method.
9. Calculate the scores.
10. Analyze the differences between the prompt patterns.
11. Prepare the final comparison report.

---

# Result

The prompts for **Zero-Shot, Few-Shot, Chain-of-Thought, Persona, Reverse, Graph, and Active Prompting** were successfully designed and evaluated for the **IoT-based smart manufacturing and predictive maintenance** use case. The rubric-based comparison demonstrated that different prompt patterns produce different types of AI responses depending on the task requirements.

