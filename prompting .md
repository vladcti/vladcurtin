---

title: "🎯 Intentional Prompting with AI: My Weather App Journey"
author: "vinesh dwarka davay"
format:
pdf:
toc: false
colorlinks: true
docx:
toc: false
highlight-style: github
html:
toc: true
toc-expand: 2
embed-resources: true
---------------------

> Building a weather app with AI isn't just about generating code — it's about **asking smarter questions** that lead to cleaner, safer, and more Pythonic solutions.

---

## 🧠 What Is Intentional Prompting?

**Intentional prompting** means I:

* Asked the AI to **explain** each code choice (e.g. why use try/except or how API responses are structured)
* Refined my prompts to move from raw responses to user-friendly output
* Questioned and improved the code AI provided instead of blindly copying
* Treated the AI like a **coding partner**, not a shortcut

---

## 💬 Smart Prompts I Used (or Improved Upon)

| Goal                 | Prompt                                                                        |
| -------------------- | ----------------------------------------------------------------------------- |
| Simplify output      | "How do I extract just the temperature and condition from this API response?" |
| Handle bad input     | "Can you show me how to add error handling if the weather keys are missing?"  |
| Format output nicely | "How do I use emojis and formatting to make the printout more readable?"      |
| Improve reliability  | "What’s the best way to add a timeout to the requests call?"                  |
| Add features         | "Can you help me include a forecast for the next few days too?"               |

---

## 🧩 Prompting In Action: From Basic to Better

### ❌ Lazy Prompt:

> "Write a weather app in Python."

**Result:** A generic script that returns the entire raw JSON — too much data, poor UX.

### ✅ Intentional Prompt:

> "Write a Python function that returns only the temperature and condition for a location, with error handling and a readable format."

**Result:** Clean output, well-structured function, safe from crashes.

---

## 🧠 Debugging and Improving with AI

Even good AI responses had gaps:

* The API might fail → I asked, *"Can you add try/except blocks?"*
* The response had too much info → I followed up, *"How do I just get today’s condition?"*
* The code lacked documentation → I requested a docstring and clearer naming

This back-and-forth led to a **more robust, readable** app.



## 🔄 Prompting Is a Process

I didn’t get the perfect code in one go. I:

1. Started with a general idea
2. Tested the output
3. Saw issues (missing keys, formatting, UX)
4. Re-prompted for better code or explanation

Just like debugging — prompting well is an iterative Python skill.



## 🧳 Final Tip: Track Your Prompting Wins

I logged prompts like:

* How to filter weather data
* How to log to a file safely
* How to expand the output to a forecast

This not only shows growth, but also proves that I can use AI **intentionally and effectively** as a Python developer.



> In the end, it wasn’t about the AI doing the coding for me  it was about **learning to think better** with AI.
