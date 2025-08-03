# Automated-Book-Rewriting-Workflow-using-AI-Reinforcement-Feedback-ChapterForge-

# ChapterForge – Human-in-the-Loop AI Book Rewriting Pipeline

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

bash
Copy
Edit
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



 🙋 Author
Name:Himani Barmase
Email: himanibarmase111@gmail.com
