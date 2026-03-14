---
layout: article
title: QBLink
---

# QBLink: Sequential Open-Domain Question Answering

QBLink is a dataset for sequential question answering where multiple related questions about the same topic are answered in sequence. It evaluates how well QA systems leverage context from previous questions and answers.

**18,644 sequences · 56,000 question–answer pairs**

## Dataset Structure

Each sequence contains:

| Field | Description |
|---|---|
| `id` | Sequence identifier |
| `tournament` | Quiz bowl tournament source |
| `lead-in` | Introductory sentence defining the topic |
| `category` | Subject area (History, Literature, Philosophy, etc.) |
| `sub-category` | More specific classification |
| Questions 1–3 | Each with `question_text`, `raw_answer`, `wiki_page` |

Example sequences cover topics such as Bitcoin's inventor or Ronald Reagan's presidency, where later questions reference earlier answers to test contextual reasoning.

## Download

| Split | File |
|---|---|
| Train | [QBLink-train.json](https://drive.google.com/file/d/1OFNQcxv8l1R0xOrmz6mKqBfECBHBB_Yx/view) |
| Dev | [QBLink-dev.json](https://drive.google.com/file/d/1OFNQcxv8l1R0xOrmz6mKqBfECBHBB_Yx/view) |
| Test | [QBLink-test.json](https://drive.google.com/file/d/1OFNQcxv8l1R0xOrmz6mKqBfECBHBB_Yx/view) |

## Citation

> Ahmed Elgohary, Chen Zhao, Jordan Boyd-Graber.
> **Dataset and Baselines for Sequential Open-Domain Question Answering.**
> *EMNLP 2018.*

## Authors

- Ahmed Elgohary — elgohary@cs.umd.edu
- Chen Zhao — chenz@cs.umd.edu
- Jordan Boyd-Graber — jbg@cs.umd.edu
