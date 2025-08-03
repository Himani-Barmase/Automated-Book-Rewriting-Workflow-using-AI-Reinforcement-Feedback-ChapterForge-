# Automated-Book-Rewriting-Workflow-using-AI-Reinforcement-Feedback-ChapterForge-



## 📘 Project Purpose

ChapterForge is a structured content rewriting pipeline that combines web scraping, text generation, review, and semantic storage to automate the creative rewriting of book chapters. The workflow includes multiple iterations with human feedback to simulate a reinforcement learning (RL)-like reward system for improving the quality of rewritten content.

---
## 🔧 Key Features

- ✅ Scrapes chapter text from public domain sources like Wikisource.
- ✅ Option to extract chapter content from uploaded PDFs.
- ✅ Rewrites chapters using open-source large language models (LLMs).
- ✅ Simulates AI reviews and supports manual human feedback.
- ✅ Stores and compares chapter versions using ChromaDB and sentence embeddings.
- ✅ Tracks ratings, feedback, and rewritten outputs across multiple iterations.

---

## 📂 Project Structure

ChapterForge/
│
├── chapterforge.py # Main project script
├── requirements.txt # Python dependencies
├── feedback_log.txt # Stores feedback for each iteration
├── rewritten_output_v1.txt # Rewritten chapter version 1
├── rewritten_output_v2.txt # Rewritten chapter version 2
├── rewritten_output_v3.txt # Rewritten chapter version 3

Install dependencies
Install dependencies


pip install -r requirements.txt
Run the script step-by-step
Launch in Jupyter/Colab or run directly with Python:


python chapterforge.py
Rate and give feedback
During each iteration, provide feedback (1–5) and comments that are used to adjust the rewrite prompt for the next version.

Check output files
Find all rewritten versions and logs in the root directory.

🧠 Technologies Used
requests, beautifulsoup4 – Scraping content from Wikisource

PyPDF2 – Parsing content from PDFs

transformers, torch – Language models for rewriting and review

sentence-transformers, chromadb – Semantic version control

ChromaDB – Embedding storage and search


 Project Overview

What it is:

An AI-powered workflow that scrapes book chapters, rewrites them creatively using large language models, refines them through human and AI feedback, and tracks versions with semantic search — all enhanced with a reinforcement learning-style loop.

Why it’s useful:

It reduces manual rewriting effort, improves creative quality via feedback, and introduces automation into editorial pipelines for writers, editors, and publishers.

How it helps:

It provides a structured, repeatable system for producing high-quality, AI-assisted content with human oversight, version control, and reward-driven iteration.

🛠️ Step-by-Step Workflow

Step 1: Scrape Chapter from Wikisource
Scrapes the content of a chapter from a public domain book URL using requests and BeautifulSoup, then saves it as a plain text file.


Step 2: Extract Text from PDF (Alternative Input Mode)

Allows users to extract chapter content from a PDF using PyPDF2 if they prefer uploading instead of web scraping.


Step 3: AI Rewriting of Chapter (AI Writer)

Uses Hugging Face language models like GPT-2, Falcon, or GPT-Neo to rewrite the text in a more vivid, novel-style format without changing its meaning.


Step 4: AI Review & Scoring (AI Reviewer)

A sentiment or classification model simulates reviewing the rewritten content based on storytelling quality, clarity, and vocabulary, assigning a star rating.


Step 5: Human-in-the-Loop Feedback
Displays the AI-generated output to a human who rates the text (1–5 stars) and provides qualitative feedback used in the next rewrite cycle.


Step 6: RL-Based Iterative Rewriting

Simulates a reinforcement learning loop by adjusting the prompt based on human feedback and re-generating improved versions of the chapter in multiple iterations.


Step 7: Semantic Version Control with ChromaDB
Stores each rewritten version in a vector database using ChromaDB and SentenceTransformers, allowing semantic search and retrieval of similar or better versions.


Step 8: Agent Pipeline (Writer → Reviewer → Editor)

Implements a modular AI agent flow: the Writer rewrites, the Reviewer scores, and the Editor optionally refines grammar or structure. Each agent functions independently.


Step 9: Export Rewritten Versions

Saves each iteration (v1, v2, v3) of the rewritten chapter to text files for download and comparison, preserving the creative history of the content.


Step 10: Feedback Logging for Reward Loop

Appends every feedback and rating from the human reviewer into a feedback_log.txt file for auditability, tracking improvement, and future model fine-tuning.


Step 11: Semantic Search for Past Versions

Enables searching for previous rewritten chapters that are similar in meaning but different in wording, using vector similarity — useful for refining or comparing styles.



 🙋 Author
Name:Himani Barmase
Email: himanibarmase111@gmail.com
