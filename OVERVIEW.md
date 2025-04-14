# 🧱 Mini Hello API in Python (Flask)

## Overview

This is a simple walkthrough of setting up a basic REST API using Python and Flask, including environment setup and pushing to GitHub.

---

## Steps

### Step 1: Create a Project Folder

```bash
mkdir hello-api
cd hello-api
```

### Step 2: Create Virtual Environment

```bash
python -m venv venv
```

- **Activate (Windows):**

```bash
venv\Scripts\activate
```

- **Activate (Mac/Linux):**

```bash
source venv/bin/activate
```

### Step 3: Install Flask

```bash
pip install Flask
```

### Step 4: Create `app.py`

```python
from flask import Flask
app = Flask(__name__)

@app.route('/')
def hello():
    return "Hello, World!"

if __name__ == '__main__':
    app.run(debug=True)
```

### Step 5: Run the App

```bash
python app.py
```

Visit: `http://127.0.0.1:5000/` to see `Hello, World!`

---

## Step 6: Initialize Git

```bash
git init
git add .
git commit -m "Initial commit"
```

---

## Step 7: Push to GitHub

### First Time:

```bash
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

### If You Created a README on GitHub First:

Error: `Updates were rejected because the remote contains work...`

**Fix:**

```bash
git pull origin main --allow-unrelated-histories
git add .
git commit -m "Merge remote-tracking branch 'origin/main'"
git push -u origin main
```

---

# 🔹 Git Cheat Sheet

| Action                  | Command                                            |
| ----------------------- | -------------------------------------------------- |
| Initialize Repo         | `git init`                                         |
| Stage Files             | `git add .`                                        |
| Commit Changes          | `git commit -m "message"`                          |
| Add Remote              | `git remote add origin URL`                        |
| Push to Remote          | `git push -u origin main`                          |
| Pull from Remote        | `git pull origin main`                             |
| Fix Unrelated Histories | `git pull origin main --allow-unrelated-histories` |
| List Git Status         | `git status`                                       |
| Log Commits             | `git log`                                          |

---

## Done! 🎉

You can now add this `README.md` to your GitHub repository to document your mini Hello API project.

Let me know when you want help for your next one!

