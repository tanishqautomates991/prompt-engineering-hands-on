# Prompt Engineering Assessment — Prompt Library

This document contains the **Before (Naive)** and **After (Optimized)** prompts for six marketing content types. The optimized prompts are intentionally beginner-friendly and focused on practical prompt engineering rather than over-engineering.

---

## Task 1 — Blog Post

### Technique
**RGCCO Framework + Style Transfer**

### Variables
`[Topic]`, `[Reference Text]`

### Before — Naive Prompt

```text
Write a blog post about why remote work is good.
```

### After — Optimized Prompt

```text
Role:
You are an experienced blog writer.

Goal:
Write an informative blog post about why remote work is good.

Context:
The target audience is B2B managers and business professionals. Explain the practical benefits of remote work in a clear and useful way.

Constraints:
- Use active voice and simple language.
- Avoid corporate jargon and unnecessary fluff.
- Use clear headings and bullet points where useful.
- Keep the article focused on practical benefits.

Style Transfer:
Write in the style of the following reference text:
[Reference Text]

Use its tone and writing style, but create original content.

Output Format:
- H1 title
- H2 headings
- Introduction
- Bullet points where appropriate
- Conclusion
```

---

## Task 2 — LinkedIn Post

### Technique
**Role Prompting + Zero-Shot with Strict Constraints**

### Variables
`[Theme]`, `[Persona]`

### Before — Naive Prompt

```text
Write a LinkedIn post about learning prompt engineering.
```

### After — Optimized Prompt

```text
Role:
You are a Senior [Persona] sharing practical insights on LinkedIn.

Goal:
Write an engaging LinkedIn post about [Theme] for professionals interested in AI and career growth.

Constraints:
- Start with a strong hook.
- Keep it under 150 words.
- No emojis or buzzwords.
- Use a clear and professional tone.

Output Format:
Hook + short body + final takeaway or question.
```

---

## Task 3 — Email Campaign

### Technique
**Few-Shot Prompting**

### Variables
`[Offer]`, `[Examples]`

### Before — Naive Prompt

```text
Write a sales email promoting our new water bottle.
```

### After — Optimized Prompt

```text
Role:
You are a marketing copywriter.

Examples:
[Examples]

Goal:
Write a persuasive sales email for our new water bottle using the structure and tone of the examples.

Offer:
[Offer]

Constraints:
- Focus on customer benefits.
- Keep the email concise and easy to read.
- Use a clear and persuasive call to action.
- Do not copy wording from the examples.

Output Format:
Subject line + email body + CTA.
```

---

## Task 4 — Instagram Caption

### Technique
**Few-Shot Prompting**

### Variables
`[Image Description]`, `[Examples]`

### Before — Naive Prompt

```text
Write an Instagram caption for a picture of a coffee.
```

### After — Optimized Prompt

```text
Role:
You are a social media copywriter.

Image Description:
[Image Description]

Examples:
[Examples]

Goal:
Create an engaging Instagram caption that matches the mood of the coffee image and follows the useful patterns from the examples.

Constraints:
- Start with an engaging line.
- Keep it natural and relatable.
- Keep it between 50–100 words.
- Do not copy the examples or invent image details.

Output Format:
Return only the final Instagram caption.
```

---

## Task 5 — YouTube Script

### Technique
**Role Prompting + RGCCO**

### Variables
`[Goal]`, `[Topic]`

### Before — Naive Prompt

```text
Write a Youtube video script about how to start a business.
```

### After — Optimized Prompt

```text
Role:
You are a YouTube retention strategist and script writer.

Goal:
[Goal]

Topic:
[Topic]

Context:
Create a beginner-friendly video that explains the topic clearly and keeps viewers interested.

Constraints:
- Use simple and conversational language.
- Avoid unnecessary jargon and filler.
- Start with a strong hook.
- Keep the information practical and easy to follow.

Output Format:
1. 0–30s: Hook
2. Main content in clear steps
3. Short CTA
```

---

## Task 6 — Product Description

### Technique
**Feature-to-Benefit Mapping + Constraints**

### Variables
`[Specs]`, `[Examples]`

### Before — Naive Prompt

```text
Write a product description for a wireless mouse.
```

### After — Optimized Prompt

```text
Role:
You are an e-commerce product copywriter.

Product Specifications:
[Specs]

Examples:
[Examples]

Goal:
Write a clear product description for the wireless mouse and turn each important feature into a useful customer benefit.

Constraints:
- Explain features in simple language.
- Focus on practical user benefits.
- Do not make unsupported claims.
- Avoid exaggerated marketing language.

Output Format:
Short product description + Features → Benefits + CTA.
```

---

## Summary

| Task | Content Type | Technique | Variables |
|---|---|---|---|
| 1 | Blog Post | RGCCO + Style Transfer | `[Topic]`, `[Reference Text]` |
| 2 | LinkedIn Post | Role Prompting + Zero-Shot | `[Theme]`, `[Persona]` |
| 3 | Email Campaign | Few-Shot Prompting | `[Offer]`, `[Examples]` |
| 4 | Instagram Caption | Few-Shot Prompting | `[Image Description]`, `[Examples]` |
| 5 | YouTube Script | Role Prompting + RGCCO | `[Goal]`, `[Topic]` |
| 6 | Product Description | Feature-to-Benefit + Constraints | `[Specs]`, `[Examples]` |
