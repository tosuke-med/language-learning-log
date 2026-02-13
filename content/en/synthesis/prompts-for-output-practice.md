---
title: Prompts for Output Practice with LLMs
date: 2026-02-14
language: en
tags: [prompts, speaking, writing, LLM]
---

This page summarizes the prompts and techniques for practicing English output using Large Language Models (LLMs), based on my learning logs.

## The Challenge

LLMs are great at generating text, but this creates a problem for language learners: **they tend to give you the answer before you have a chance to practice**. When you want to practice using a phrase in context, the LLM often shows you a model sentence first, which defeats the purpose of active recall.

The prompts below are designed to solve this problem.

---

## Prompt 1: Situation-Based Practice (Writing/Speaking)

This prompt is for practicing phrases through realistic situations. The key feature is the **hidden phrase pool** — the LLM knows the phrases but never reveals them until after you answer.

### How It Works

1. You paste a list of phrases you want to practice
2. The LLM treats them as a hidden pool
3. For each phrase, it presents a situation where the phrase would be useful
4. You respond without seeing the phrase
5. The LLM gives feedback and reveals the reusable pattern

### The Prompt

```
## Goal
Practice **recalling and using reusable key expressions and patterns** from target English phrases **naturally in context**, **without being shown the phrases in advance**.

## Initial Step
- I will paste a **list of phrases all at once**.
- Treat these phrases as a **hidden phrase pool**.
- **Do not**:
  - show
  - number
  - quote
  - hint at
  any of the phrases at this stage or during practice.

## Core Rules
- For each round:
  - Randomly select **one phrase internally** from the hidden pool.
  - Keep the selected phrase **completely hidden until feedback**.
- **Never reveal the phrase before my first answer**.
- My answer **does not need to reproduce the full phrase**.
- **Prioritize naturalness and communicative effectiveness** over phrase matching.

## Practice Flow
*(Repeat for each hidden phrase)*

### 1. You
- Present **only a natural situation** where
  some **part, pattern, or idea** from the hidden phrase could be used.
- **No model sentences**
- **No example answers**

### 2. Me
- I answer in English (**1–2 sentences**).

### 3. You — Feedback (TWO parts)

#### (a) General Feedback
- Evaluate how natural my answer is **on its own**.
- Provide a **revised version** of my answer.

#### (b) Expression-Based Feedback
- Explain which **key expression, structure, or wording pattern** from the hidden phrase could be useful in this situation.
- You **may reveal the full phrase here only as a source**, not as a memorization target.
- Explicitly point out the **reusable part**
  (e.g. a clause, collocation, or framing).
- Provide **one example answer** that uses the reusable part
  (not necessarily the full phrase).

### 4. You
- Present **another situation** where the **same reusable expression or pattern**
  (from the same hidden phrase) could be applied.
- **No model sentences**
- **No example answers**

### 5. Me
- I answer again.

### 6. You — Feedback
- Use the **same two-part format** as above.

### 7. Transition
- Move on to a **new hidden phrase**.
- Repeat the cycle.
```

---

## Prompt 2: Conversational Practice

This prompt focuses on natural conversational exchanges. Instead of just presenting situations, the LLM acts as a conversation partner.

### How It Works

1. The LLM starts a conversation based on a hidden phrase
2. You respond naturally (you don't need to use the target phrase)
3. The LLM replies as a conversation partner
4. After a short exchange, you get feedback on both naturalness and expression usage

### The Prompt

```
## Goal
Practice reusing idioms, expressions, and wording patterns from target English phrases through short, natural conversational exchanges, without seeing the phrases in advance.

## Initial Step
I will paste a list of phrases all at once.
Treat them as a hidden phrase pool.
Do not show, quote, number, or hint at the phrases during practice.

## Core Rules
- Select one hidden phrase per mini-conversation
- Focus on reusable parts of the phrase (idioms, collocations, framing), not the full sentence
- Prioritize natural conversational flow over phrase matching
- Never reveal the phrase before feedback

## Practice Flow (repeat for each hidden phrase)

### You
Present a natural conversational situation.
Act as the other speaker and respond naturally to me.
No model sentences. No example answers.

### Me
Respond in English (1 sentence).

### You
Reply as the conversation partner (1 sentence).

### Me
Respond again (1 sentence). <-- I don't need to use the expression here.

### You — Feedback
Provide two parts only:

**(a) Conversation feedback**
- Briefly evaluate the naturalness of the exchange
- Provide a clean revised version of my replies only

**(b) Expression-based feedback**
- Reveal the source phrase
- Explicitly point out the reusable part (idiom / structure / wording)
- Explain how it fits the conversation
- Give one short example line using that reusable part
```

---

## Why These Prompts Work

### 1. Two Situations Per Phrase
Each phrase is practiced in **two different contexts**. This helps you generalize the expression rather than memorizing it for just one situation.

### 2. Focus on Reusable Parts
The prompts emphasize **reusable patterns** (collocations, structures, framing) rather than full sentences. This makes the phrases more flexible and applicable.

### 3. Stimulus-Response Connection
In real communication, we speak in response to stimuli — visual cues, contexts, or what someone just said. These prompts simulate that by presenting situations first, then asking you to respond.

### 4. No Premature Answers
The strict "hidden phrase" rules prevent the LLM from spoiling your practice by showing answers too early.

---

## Tips for Using These Prompts

- **Start simple**: Begin with 5-10 phrases per session
- **Mix sources**: Include phrases from different contexts (news, novels, academic writing)
- **Review regularly**: Weekend review sessions help consolidate learning
- **Adapt for your level**: At higher levels (B2-C1+), you may need more abstract and nuanced situations

---

## Related Techniques

### Kindle + LLM for Reading
Highlight unfamiliar expressions while reading on Kindle, then paste them into an LLM for explanation. This preserves reading flow while enabling later review.

### News + LLM for Context
News headlines often contain specialized idioms (e.g., legal terms like "seek damages"). LLMs excel at explaining these context-dependent expressions.

### NotebookLM for Listening Review
After online English lessons, upload the audio recording to [Google NotebookLM](https://notebooklm.google/) to get a transcript for review.

---

*These prompts were developed through trial and error in my daily English learning practice. Feel free to adapt them to your own needs.*
