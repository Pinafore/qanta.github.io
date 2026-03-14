---
layout: article
title: How to Stump a Computer
---

# How to Stump a Computer

Can you write a question that a top computer QA system can't answer — but an expert human can?

Our adversarial question writing interface at **[write.qanta.org](http://write.qanta.org)** provides real-time feedback as you write. The system highlights words it finds important, helping you find clues that fool the machine.

## What Makes a Question Adversarial?

Good adversarial questions:

- **Paraphrase** rather than quote standard clues
- **Require multi-hop or logical reasoning** across multiple facts
- **Demand commonsense or expert knowledge** not in typical training data
- **Include mathematical elements** that require calculation
- **Use cross-lingual references** — names or terms from other languages

## What Makes a Question Bad?

Avoid:
- **Vague location questions** — "this country in Southeast Asia" without disambiguation
- **False presuppositions** — assuming incorrect facts (e.g., about flamingo coloring or electrical voltage)
- **Subjective specificity** — adding qualifiers that penalize knowledge rather than test it
- **"Swerve" questions** — redirecting expectations mid-question in ways that feel unfair rather than clever

## What Makes a Question Good?

A good adversarial question satisfies both criteria:
1. A knowledgeable human immediately recognizes the correct answer
2. The AI system fails to answer correctly

The answer should always be verifiable with a Wikipedia page title.

## Frequently Asked Questions

**What difficulty level should I target?**
"At least 2-dot" difficulty — roughly comparable to high school nationals (HSNCT). First 1–2 lines should be unanswerable by baseline AI.

**How do I know if my question stumps the computer?**
The interface gives live feedback — if the system doesn't highlight your answer in the top results, you're on the right track.

**What answer formats are accepted?**
Answers must correspond to Wikipedia page titles. Redirects and common alternate names are accepted.

**Can I write about any topic?**
Yes, though some answers may not be in the system's knowledge base. The interface will indicate if an answer is recognized.

## Get Started

Write questions at [write.qanta.org](http://write.qanta.org) or read about the [Adversarial QA project](/research/projects/adversarial/) for background on the research.
