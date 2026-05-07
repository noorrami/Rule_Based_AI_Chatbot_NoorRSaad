# 🤖 DecodeLabs Internship – Project 1: Rule-Based AI Chatbot

> **A deterministic, white‑box conversational agent built with pure Python logic. No deep learning, no black boxes – just control flow, hash maps, and clean decision‑making.**

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 📌 Project Overview

This is my first project as an AI Engineering Intern at **DecodeLabs**.  
The goal was to build a **rule-based chatbot** that responds to user inputs using explicit `if-else` logic (implemented via dictionaries for efficiency).  
The project demonstrates mastery of:

- **Control flow** (infinite loop, exit commands)
- **Deterministic logic** (every input maps to a predictable output)
- **Input sanitisation** (lowercase, punctuation removal, whitespace trimming)
- **Hash map lookups** (O(1) performance instead of long if‑elif chains)
- **Keyword matching** for flexible, natural interactions
- **User personalisation** (remembers and uses the user's name)

> 🔍 *“Before you can manage the chaos of a probability engine, you must master the precision of a logic engine.”* – DecodeLabs

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🧠 **Pure rule‑based** | No ML, no APIs – just Python dictionaries and conditionals. |
| 📝 **Personalised replies** | Asks for your name at the start and includes it in every response. |
| 🔍 **Exact + keyword matching** | Understands full commands (`"how are you"`) and keywords inside sentences (`"tell me about python"`). |
| 🎲 **Randomised responses** | Multiple possible replies per intent; chosen randomly to avoid repetition. |
| 🧹 **Input sanitisation** | Handles uppercase, punctuation, extra spaces gracefully. |
| 🚪 **Clean exit** | Type `bye`, `exit`, `quit`, or `goodbye` to end the conversation. |
| 📋 **Built‑in help** | `help` command lists all available intents. |

---

## 🗂️ Knowledge Base (Intents)

The chatbot recognises the following **exact intents** (and many more via keywords):

- `hello`, `hi`, `hey` → Greetings
- `how are you`, `how are you doing` → Well‑being
- `what is your name`, `who are you` → Bot identity
- `what is my name` → Recalls your name
- `time`, `date` → Mock responses
- `thanks`, `thank you` → Appreciation
- `yes`, `no` → Affirmative / negative
- `help` → Command list
- `bye`, `exit`, `quit`, `goodbye` → Exit

**Keyword‑based intents** (triggered anywhere in a sentence):

- `weather`, `rain`, `love`, `hate`, `python`, `code`, `robot`, `smart`, `dumb`, `food`, `fun`

---

## 🚀 How to Run

### Prerequisites
- Python 3.8 or higher installed on your machine.

### Steps

1. **Clone the repository** (or download the script `chatbot.py`):
   ```bash
   git clone https://github.com/YOUR_USERNAME/DecodeLabs-Internship.git
   cd DecodeLabs-Internship
