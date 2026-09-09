# 🤖 AI-Powered Learning & Personalized Study Assistant

An AI-powered educational assistant designed to help students learn, practice, and track their progress using **Retrieval-Augmented Generation (RAG), Memory, and Tool Calling**.

---

## 📌 Project Overview

The **AI Learning & Personalized Study Assistant** helps students interact with their own study materials and receive personalized learning support.

Students can upload PDF study materials, ask questions, generate quizzes, create study plans, and track their learning progress.

The system combines:

- 📚 Retrieval-Augmented Generation (RAG)
- 🧠 Student Memory
- 🛠️ Tool Calling
- 🤖 Generative AI
- 📝 Quiz Generation
- 📅 Personalized Study Planning
- 📊 Progress Tracking

---

## ✨ Features

### 📚 1. Study Material Upload

Students can upload PDF files containing:

- Lecture notes
- Study materials
- Syllabus
- Textbooks
- Subject notes

The system extracts the text and uses it to provide context-aware answers.

### 🤖 2. AI Tutor

Students can ask questions related to their uploaded study material.

The AI provides answers based on the relevant information retrieved from the documents.

### 🧠 3. Student Memory

The system maintains lightweight student learning memory, including:

- Student name
- Subject
- Preferred difficulty
- Quiz scores
- Weak topics
- Learning history

### 📝 4. Quiz Generator

The assistant can generate quizzes based on the student's subject or uploaded study materials.

### 📅 5. Personalized Study Plan

The system generates study plans based on the student's learning requirements and weak areas.

### 📊 6. Progress Tracking

Students can track:

- Quiz attempts
- Quiz scores
- Average performance
- Weak topics
- Learning progress

### 🎯 7. Weak Topic Identification

The system records topics where the student needs additional practice and uses this information for personalized learning.

---

# 🏗️ System Architecture

```text
                    👩‍🎓 Student
                         │
                         ▼
                 🖥️ Gradio Interface
                         │
          ┌──────────────┴──────────────┐
          │                             │
          ▼                             ▼
    📄 PDF Upload                 ❓ Student Question
          │                             │
          ▼                             ▼
   Text Extraction              🔍 Information Retrieval
          │                             │
          └──────────────┬──────────────┘
                         ▼
                  📚 Relevant Context
                         │
                         ▼
                  🤖 Gemini AI
                         │
              ┌──────────┼──────────┐
              │          │          │
              ▼          ▼          ▼
           🧠 Memory   🛠️ Tools   📊 Progress
              │          │          │
              └──────────┼──────────┘
                         ▼
               💬 Personalized Response
