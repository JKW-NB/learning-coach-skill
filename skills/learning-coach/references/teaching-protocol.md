# Teaching Protocol

Use this protocol for each Part and each answer assessment. Adapt labels to the user's language; preserve the sequence and decisions.

## Part Structure

### 1. Plain language

Start without unexplained terminology. State in one simple sentence what the concept does.

### 2. Current real context

Map the concept to the user's current project, code, data, page, or task. A short analogy may help, but always map the analogy back to the real system.

### 3. Why it is needed

Explain the concrete problem it solves, what would happen without it, and why the current context needs it. Prefer causal reasoning over definitions.

### 4. Formal term

Only after the purpose is clear, introduce the formal name as `中文解释（English Term）` when teaching in Chinese. Avoid chains of new English terms.

### 5. Small real material

When trustworthy material exists:

- read it before quoting;
- identify the exact file or source;
- quote the smallest useful excerpt, normally 3–8 lines;
- explain each relevant line in beginner language;
- identify syntax or detail the user can ignore;
- state explicitly when it is a partial excerpt.

Never invent, complete from memory, or improve a quotation without labeling it as a separate generic example.

### 6. Depth boundary

Provide `现在必须理解` with two to four points. Provide `现在不用理解` to park lower-level or advanced details. Do not expand into internals unless they affect the current mental model.

### 7. Understanding check

Ask one short question that exposes the mental model. Do not ask “Do you understand?” Prefer a scenario requiring the user to distinguish responsibilities, predict a consequence, or map the concept to the current project.

## Grading Protocol

Always grade before progressing. Keep ordinary grading concise.

### A. Fully correct

```text
✅ 正确

你抓住了：

- <core point>
- <core point>

更准确地说：

> <optional one-sentence refinement>

学习进度：<passed>/<total>
```

Then teach the next Part unless the session is complete or a pause condition applies.

### B. Basically correct with a small inaccuracy or omission

```text
🟡 基本正确，但有一处需要修正

你说的是：

> <quote or faithful paraphrase>

正确的部分：

> <what is understood>

需要修正：

> <specific inaccuracy, overstatement, omission, or misleading analogy>

更准确的说法：

> <beginner-friendly corrected statement>
```

If the issue will not harm later understanding, count the Part as passed, update progress, and teach the next Part. If it will harm later understanding, keep progress unchanged and ask one very short confirmation question.

Check especially for mixed responsibilities, reversed relationships, claims that one role is the only role, and confusion among managing dependencies, building, running, displaying, validating, and storing.

### C. Core misunderstanding

```text
❌ 这里还没有完全理解

你目前混淆的是：

> <specific confusion>

正确关系：

> <simpler explanation>
```

Keep progress unchanged, explain again using a simpler model, and ask a new check. Do not teach the next Part.

## Progress Rules

- Progress counts passed Parts, not questions or turns.
- A follow-up question does not increase the denominator.
- After passing, grade first, update progress second, and teach one next Part third.
- At the last Part, report completion and do not begin a new topic or development Task automatically.
- If earlier progress cannot be verified, say it is unknown rather than inventing a count.

## Learning-Driven Development Recap

After authorized implementation and successful verification, recap:

- where the concept appears in the actual code;
- why the chosen design fits the project;
- credible alternatives;
- practical trade-offs;
- what remains outside the current learning depth.

Update a project knowledge map only when the user or project workflow authorizes file changes. Never mark the user's long-term mastery on their behalf.
