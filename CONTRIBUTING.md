# Contributing to CampusConnect

Welcome to the **CampusConnect Project** 🎓

This guide explains step by step how students of the **Xonovate Code Champions Apprenticeship 2025 Cohort** can set up and contribute to the project.

---

## 0️⃣ Step 0 – Install Python and Git (If Not Already Installed)

Before you start, make sure you have **Python 3.10 or higher** and **Git** installed on your computer.
These tools are required to run Django 5 and manage project version control.

### 🐍 Check Your Python Version

Open your terminal or command prompt and run one of the following commands:

```bash
python --version
```

or

```bash
python3 --version
```

You should see something like:

```
Python 3.10.x  (or above)
```

If you don’t have Python or your version is below **3.10**, download and install the latest version from:
👉 [Download Python](https://www.python.org/downloads/)

After installation, close and reopen your terminal, then check the version again to confirm.

### 💻 Check Your Git Installation

Run this command to check if Git is installed:

```bash
git --version
```

If it shows a version number, you’re good to go.
If not, install Git from:
👉 [Download Git](https://git-scm.com/downloads)

After installing both, restart your terminal before continuing.

---

## 1️⃣ Step 1 – Fork the Repository

Go to the main CampusConnect repository:
👉 [https://github.com/xonovate-codechampions/CampusConnect](https://github.com/xonovate-codechampions/CampusConnect)

Click **Fork** (top-right corner).
This creates a copy of the project under your own GitHub account.

---

## 2️⃣ Step 2 – Clone Your Fork

Open your terminal (or VS Code terminal) and run:

```bash
git clone https://github.com/YOUR-GITHUB-USERNAME/CampusConnect.git
```

Replace `YOUR-GITHUB-USERNAME` with your GitHub username.
Then move into the project folder:

```bash
cd CampusConnect
```

---

## 3️⃣ Step 3 – Create a Virtual Environment

A **virtual environment** keeps all the project’s Python packages separate from your global Python installation.
It ensures everyone is using the same versions of dependencies.

You can learn more here:
📘 [What is a Python Virtual Environment and Why You Need It](https://realpython.com/python-virtual-environments-a-primer/)

Now, create your environment.

### Windows:

```bash
python -m venv venv
```

### macOS/Linux:

```bash
python3 -m venv venv
```

---

## 4️⃣ Step 4 – Activate the Virtual Environment

### Windows:

```bash
venv\Scripts\activate
```

### macOS/Linux:

```bash
source venv/bin/activate
```

Once it’s activated, you should see `(venv)` at the beginning of your terminal line.

---

## 5️⃣ Step 5 – Install Project Requirements

Install all the required dependencies listed in `requirements.txt`:

```bash
pip install -r requirements.txt
```

If you see any errors during installation, ask for help before continuing.

---

## 6️⃣ Step 6 – Apply Database Migrations

Run the following commands one after the other to prepare the database:

```bash
python manage.py makemigrations
```

```bash
python manage.py migrate
```

This creates all necessary tables for Django to run.

---

## 7️⃣ Step 7 – Run the Development Server

Start the project to make sure everything works.

### Windows:

```bash
python manage.py runserver
```

### macOS/Linux:

```bash
python3 manage.py runserver
```

Then open your browser and visit:

```
http://127.0.0.1:8000/
```

You should see the CampusConnect homepage 🎉

---

## 8️⃣ Step 8 – Picking a Task (Issues Workflow)

All tasks and features will be listed as **Open Issues** on the repository’s **Issues** tab.
👉 [View CampusConnect Issues](https://github.com/xonovate-codechampions/CampusConnect/issues)

### How to work on an issue:

1. Go to the **Issues** tab in the repo.
2. Read through the open issues carefully.
3. Pick one that interests you or has been assigned to you.
4. Comment on the issue saying, “I’ll work on this,” so others know it’s taken.
5. Once approved, create your branch for that issue and start working on it.

Example branch name:

```bash
git checkout -b feature/add-login-page
```

---

## 9️⃣ Step 9 – Make Your Changes

Now open the project in **VS Code** and start working on your assigned task.
Make sure your changes are:

- Neatly indented
- Well commented
- Relevant to your assigned issue

---

## 🔟 Step 10 – Save and Commit Your Work

When done:

```bash
git add .
git commit -m "Added login page structure"
```

Your commit message should describe what you changed.

---

## 11️⃣ Step 11 – Push Your Branch to GitHub

Send your changes to your own repository:

```bash
git push origin feature/add-login-page
```

---

## 12️⃣ Step 12 – Open a Pull Request

Go to your GitHub repository, and you’ll see:

> “Compare & Pull Request”

Click it, write a short description of what you did, and submit the **Pull Request** for review.

---

## 13️⃣ Step 13 – Keep Your Fork Updated

When the main project is updated, pull the latest changes.

```bash
git checkout main
git pull https://github.com/xonovate-codechampions/CampusConnect.git main
```

Then continue your work from an updated codebase.

---

## ✅ Summary of All Steps

0. Install Python 3.10+ and Git
1. Fork the repo
2. Clone your fork
3. Create and activate a virtual environment
4. Install requirements
5. Run migrations
6. Start the server
7. Pick a task from the Issues tab
8. Create your branch
9. Make your changes
10. Commit and push
11. Create a pull request
12. Keep your fork updated

---

## 💡 Tips for All Apprentices

- Always work in your own branch.
- Make one clear change per pull request.
- Check the **Issues tab** for what to work on next.
- Ask questions if you’re unsure — this is a learning process.
- Keep your environment active while running the project.

---

## 📘 Additional Resources

- [Install Python](https://www.python.org/downloads/)
- [Install Git](https://git-scm.com/downloads)
- [GitHub Docs: Creating a Branch](https://docs.github.com/en/get-started/using-git/about-branches)
- [Django Migrations Explained](https://docs.djangoproject.com/en/stable/topics/migrations/)
- [Python Virtual Environments (Real Python)](https://realpython.com/python-virtual-environments-a-primer/)

---

**CampusConnect – Built by Students. For Students.**
Part of the **Xonovate Code Champions Apprenticeship 2025 Cohort**
