# Prompting Techniques

## 1. Zero-shot Prompting

The model is given only the task without any examples.

### Example

```text
Write a C# method to reverse a string.
```

---

## 2. Few-shot Prompting

The prompt includes one or more examples to guide the model.

### Example

```text
Input: 4
Output: 16

Input: 5
Output: 25

Input: 8
Output:
```

---

## 3. Chain-of-Thought Prompting

The prompt encourages the model to reason through the problem step by step before producing an answer.

### Example

```text
Solve the problem step by step and explain your reasoning before giving the final answer.
```

## Comparison

| Technique | Uses Examples | Best For |
|-----------|---------------|----------|
| Zero-shot | No | Simple tasks |
| Few-shot | Yes | Pattern-based tasks |
| Chain-of-Thought | Optional | Complex reasoning and problem solving |