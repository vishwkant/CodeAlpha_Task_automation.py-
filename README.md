# 📧 Email Extractor - Task Automation Script

Hey! This is a simple Python automation script I built to solve a common, repetitive problem: searching through big chunks of text to find email addresses. Instead of manually copying and pasting, this script does all the heavy lifting in seconds.

## 🚀 What This Does
The script scans a text file called `input.txt`, identifies every valid email address inside it using a specific pattern (Regular Expression), and then neatly saves all those emails into a new file called `emails.txt`.

## 🛠️ How It Works
I kept the logic straightforward so it’s easy to understand:
1.  **Reading the File:** It opens `input.txt` and reads everything inside. I added a "try/except" block so it won't crash if the file is missing—it'll just give you a friendly reminder to create it.
2.  **The "Magic" Pattern:** It uses a Regular Expression (Regex) pattern: `[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}`. This basically tells Python to look for something that has characters, an `@` symbol, a domain name, and a valid ending like `.com` or `.org`.
3.  **Saving the Results:** Once it finds all the matches, it creates (or overwrites) `emails.txt` and writes each email on its own line.

## 📋 Requirements
- Just **Python** installed on your computer.
- No extra libraries are needed because it uses `re` (built-in).

## 🏃‍♂️ How to Run It
1.  Place your text (articles, lists, notes) into a file named `input.txt`.
2.  Open your terminal or command prompt in this folder.
3.  Run the command:
    ```bash
    python task_automation.py
    ```
    *(Note: Use `py task_automation.py` if you are on Windows and the first command doesn't work!)*
4.  Open `emails.txt` to see your results!

## ✨ Why This Is Useful
This is great for anyone who needs to clean up contact lists, extract leads from documents, or just organize a mess of data. It’s fast, reliable, and way better than doing it by hand!
