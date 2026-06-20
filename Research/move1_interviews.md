# MOVE 1: BE THE TOOL YOURSELF

## Research Report: API Concept Interviews

### Objective

The goal of these interviews was to determine whether learners truly understand the concept of an API or are primarily relying on memorized definitions. The interviews were designed to move beyond surface-level explanations by introducing a derivation-based follow-up question that required participants to reason about why APIs exist and what problems they solve.

---

# Interview 1

## Concept Tested

API (Application Programming Interface)

### Opening Question

"What is an API underneath the word? How does it actually work?"

### Participant Response

"My understanding is that an API is basically a way for two applications or systems to communicate with each other. One application sends a request through an API and gets back the information or action."

### Follow-up Question

"If an API is just an interface to share data, why don't we just let external applications read directly from our system's database files instead of building API endpoints? What breaks?"

### Participant Response

"I'm honestly not completely sure. If I had to think through it, I'd say one reason could be control. If external applications could read directly from our system's database, there would be less control over who can see, or who can access the data."

### Analysis

The participant demonstrated a correct surface-level understanding of APIs as communication mechanisms between systems. However, when challenged with a deeper reasoning question, they struggled to explain why an API layer is necessary.

The participant identified control and access as possible concerns but could not explain broader architectural reasons such as validation, business logic, abstraction, rate limiting, or maintainability.

### Identified Understanding Gap

The participant understands what an API does but cannot fully derive why an API layer is necessary within software architecture.

### Understanding Level

Level 2 – Can explain the purpose of an API but cannot fully explain why the design exists.

---

# Interview 2

## Concept Tested

API (Application Programming Interface)

### Opening Question

"What is an API underneath the word? How does it actually work?"

### Participant Response

"API in simple language are just connectors which take the asked data from one place to another. I see APIs like a conveyor belt in an assembly line. Each department has a specific job and the belt carries information between them."

### Follow-up Question

"If an API is just an interface to share data, why don't we just let external applications read directly from our system's database files instead of building API endpoints? What breaks?"

### Participant Response

"If API is just an interface, we don't let external apps directly access our database because they don't know what data they are supposed to take. That's why rules and protocols exist.

There are also security concerns because we should not expose database or proprietary system data directly to external applications.

API endpoints provide specific requests such as GET, POST, PUT, PATCH and DELETE. These requests tell systems what data is needed, what action should be performed, where to retrieve information from and where to send it.

When there is specificity, systems do not break and data remains secure."

### Analysis

The participant demonstrated a stronger conceptual understanding of APIs. Instead of only describing communication, they reasoned about protocols, controlled access, security, endpoint specificity, and system reliability.

The participant was able to connect API design decisions to practical consequences in software systems.

### Identified Understanding Gap

The participant understands why APIs exist for control and security but has not fully articulated the abstraction role APIs play between consumers and internal system implementation.

### Understanding Level

Level 3 – Can explain why APIs exist and reason about system behavior but does not yet demonstrate deeper architectural reasoning.

---

# Key Findings

Both participants could define APIs as communication mechanisms.

The major difference emerged when they were asked to derive why APIs exist rather than simply define them.

Participant 1 relied primarily on memorized understanding and struggled when forced to reason about consequences.

Participant 2 demonstrated a stronger mental model by connecting APIs to rules, security, controlled access, and system stability.

This suggests that traditional API definitions are insufficient indicators of understanding. A learner may correctly define an API while lacking the ability to explain the architectural problems that APIs solve.

---

# Conclusion

The interviews support the hypothesis that conceptual understanding is better measured through derivation-based questions than through definition-based questions alone.

This finding forms the basis of the Concept Check tool, which aims to identify the exact point where a learner's understanding transitions from genuine reasoning to memorized knowledge.
