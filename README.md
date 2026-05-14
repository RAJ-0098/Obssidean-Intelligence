# Obsidian Intelligence

> AI-powered multi-agent job copilot system built using Python, RAG, and LLMs.

---

## 🚀 Overview

Obsidian Intelligence is an intelligent AI system designed to analyze job opportunities and autonomously decide whether to:

- ✅ Apply
- ⭐ Save
- ❌ Skip

The project combines:

- Large Language Models (LLMs)
- Retrieval-Augmented Generation (RAG)
- Vector embeddings
- Multi-agent workflows
- Semantic similarity scoring

The goal is to move beyond traditional keyword-based matching and build a system capable of contextual reasoning and structured decision-making.

---

# 🧠 Problem Statement

Modern job searching has become overwhelming because of:

- Thousands of repetitive applications
- Poor keyword-based filtering
- Generic resume submissions
- Lack of personalized opportunity analysis

Most existing platforms focus only on recommendations and search.

Obsidian Intelligence aims to solve this by creating an AI-powered copilot that can:

- Understand job descriptions
- Analyze candidate profiles
- Score relevance intelligently
- Decide whether a role is worth pursuing
- Generate customized application materials

---

# ⚡ Core Features

## 🔍 Job Description Analysis

- Extracts important skills, requirements, and experience levels
- Understands contextual meaning using LLMs

---

## 🧩 Retrieval-Augmented Generation (RAG)

- Stores candidate profile context using vector embeddings
- Retrieves relevant information dynamically
- Enables contextual understanding instead of keyword matching

---

## 📊 Intelligent Scoring Engine

Calculates a relevance score based on:

- Skill alignment
- Experience matching
- Semantic similarity
- Preferred technologies
- Contextual fit

---

## 🤖 Multi-Agent Workflow System

The system is designed using multiple AI agents:

| Agent | Responsibility |
|---|---|
| Analyzer Agent | Understands job descriptions |
| Scoring Agent | Computes relevance scores |
| Decision Agent | Decides Apply / Save / Skip |
| Resume Agent | Generates tailored resumes |
| Action Agent | Handles automated workflows |

---

## ✍️ Resume & Cover Letter Generation

- Generates role-specific resumes
- Creates customized cover letters using LLMs
- Optimizes content for job requirements

---

# 🛠️ Tech Stack

## Core Language
- Python

## AI / LLM Stack
- OpenAI APIs
- LangChain
- HuggingFace Transformers

## Embedding & RAG
- Sentence Transformers
- FAISS Vector Database

## Backend & APIs
- FastAPI *(Planned)*

## Frontend / UI
- Streamlit *(Planned)*

---

# 🧱 System Architecture

```text
                ┌────────────────────┐
                │ Job Description     │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │ Analyzer Agent      │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │ Embedding Engine    │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │ Vector Database     │
                │ (FAISS)             │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │ Scoring Engine      │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │ Decision Agent      │
                └─────────┬──────────┘
                          │
          ┌───────────────┼───────────────┐
          ▼                               ▼
   ┌──────────────┐              ┌────────────────┐
   │ Apply        │              │ Save / Skip    │
   └──────────────┘              └────────────────┘
