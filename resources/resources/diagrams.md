# Prompt Engineering Diagrams

This document contains visual diagrams that explain the core Prompt Engineering techniques using Mermaid. GitHub automatically renders these diagrams.

---

# 1. Prompt Engineering Workflow

```mermaid
flowchart LR
    A[User Prompt] --> B[AI Model]
    B --> C[Generated Response]
```

---

# 2. Zero-Shot Prompting

```mermaid
flowchart TD
    A[User Prompt]
    A --> B["Task: Summarize this paragraph"]
    B --> C[AI Model]
    C --> D[Generated Response]
```

### Explanation

- No examples are provided.
- The AI relies entirely on its pre-trained knowledge.

---

# 3. One-Shot Prompting

```mermaid
flowchart TD
    A[One Example]
    A --> B[Actual Prompt]
    B --> C[AI Model]
    C --> D[Generated Response]
```

### Explanation

- A single example teaches the AI the expected response style.
- The AI follows that pattern for the new prompt.

---

# 4. Few-Shot Prompting

```mermaid
flowchart TD
    A[Example 1]
    B[Example 2]
    C[Example 3]

    A --> D[Actual Prompt]
    B --> D
    C --> D

    D --> E[AI Model]
    E --> F[Consistent Output]
```

### Explanation

- Multiple examples are provided.
- The AI identifies patterns and produces more consistent responses.

---

# 5. Prompt Quality Comparison

```mermaid
flowchart LR

A[Simple Prompt]
A --> B[Generic Output]

C[Detailed Prompt]
C --> D[Specific and Accurate Output]
```

### Explanation

A detailed prompt provides more context, allowing the AI to generate higher-quality responses.

---

# 6. Choosing the Right Prompt Technique

```mermaid
flowchart TD

A[Need AI Response?]

A --> B{Examples Available?}

B -- No --> C[Zero-Shot Prompting]

B -- One --> D[One-Shot Prompting]

B -- Multiple --> E[Few-Shot Prompting]
```

---

# 7. Prompt Engineering Lifecycle

```mermaid
flowchart LR

A[Write Prompt]
--> B[Submit to AI]
--> C[Receive Output]
--> D[Evaluate Response]
--> E[Improve Prompt]
--> A
```

### Explanation

Prompt engineering is an iterative process. Better prompts generally lead to better AI responses.

---

# 8. Repository Structure

```mermaid
graph TD

A[prompt-engineering-basics]

A --> B[README.md]
A --> C[Exercises]
A --> D[Resources]
A --> E[Docs]

C --> F[Exercise 1]
C --> G[Exercise 2]
C --> H[Exercise 3]
C --> I[Exercise 4]
C --> J[Exercise 5]
C --> K[Exercise 6]
C --> L[Exercise 7]
C --> M[Exercise 8]
C --> N[Exercise 9]

D --> O[prompt-techniques.md]
D --> P[diagrams.md]

E --> Q[Assignment Document]
```

---

# 9. Learning Journey

```mermaid
journey
    title My Prompt Engineering Learning Journey

    section Fundamentals
      Learned Zero-Shot Prompting: 5: Me
      Learned One-Shot Prompting: 5: Me
      Learned Few-Shot Prompting: 5: Me

    section Practice
      Solved Exercises: 5: Me
      Compared Prompts: 5: Me
      Improved Prompt Quality: 5: Me

    section Outcome
      Better Prompt Writing Skills: 5: Me
```

---

# 10. Prompt Technique Comparison

```mermaid
flowchart LR

A[Zero-Shot]
--> D[Simple Tasks]

B[One-Shot]
--> E[Style Guidance]

C[Few-Shot]
--> F[Pattern Learning & Consistency]
```

---

# Summary

| Technique | Examples Given | Best Use Case |
|------------|----------------|---------------|
| Zero-Shot Prompting | None | Simple tasks |
| One-Shot Prompting | One Example | Learning response style |
| Few-Shot Prompting | Multiple Examples | Consistent outputs and pattern recognition |
