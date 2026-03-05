# AuraHealth
📘 GIT – Proper Neat Copy Notes (With Comments & Explanation

🔹 What is Git?                                                          
Git is a Version Control System.                             
It helps you:                             
• Track code changes                             
• Work in teams                             
• Avoid overwriting each other’s work                             
• Fix mistakes                             
• Manage hackathon pressure safely                             



---

🚀 PHASE 1: First Time Setup (Initialize Project)

# 1. Initialize Git in your project folder
git init
# Creates a new local Git repository
gfi
# 2. Connect your local project to GitHub repository
git remote add origin https://github.com/username/repository.git
# Links your folder to online GitHub repo

# 3. Add all files to staging area
git add .
# Prepares all changed files to be committed

# 4. Create first commit (snapshot)
git commit -m "Initial commit: Project Setup"
# Saves your current code version

# 5. Rename branch to main (standard branch name)
git branch -M main

# 6. Push code to GitHub
git push -u origin main
# Uploads your project to GitHub


---

🚀 PHASE 2: Daily Workflow (VERY IMPORTANT)

Whenever you write new code:

git add .
# Stage new/edited files

git commit -m "Added smart login date logic"
# Save changes with proper message

git push origin main
# Upload changes to GitHub


---

🔄 PHASE 3: Getting Latest Code (Stay Synced)

If your friend pushed code and you want latest version:

git pull origin main
# Downloads and merges latest code from GitHub

✅ Pro Tip:
Always run git pull origin main before starting work.


---

🚨 PHASE 4: Handling Merge Conflicts (Hackathon Emergency)

When two people edit the same line, Git shows conflict.

Steps to Fix:

1️⃣ Run:

git pull origin main

2️⃣ VS Code will show:

Red → Incoming change

Green → Your change


3️⃣ Choose:

Accept Current Change

Accept Incoming Change

Accept Both


4️⃣ Save the file

5️⃣ Then run:

git add .
git commit -m "Fixed merge conflict"
git push origin main


---

📌 PHASE 5: Important Commands Summary

Situation	Command

I wrote new code	git add . → git commit -m "message" → git push
I want latest code	git pull origin main
I don't know what's happening	git status
Undo last local change	git checkout .



---

📂 PHASE 6: Clean Project Structure (Recommended)

/root
 ├── /public          (Images, assets)
 ├── /src
 │    ├── /components (Login.js, Navbar.js, etc.)
 │    ├── /styles     (CSS / Tailwind)
 │    └── App.js      (Main routing)
 ├── package.json     (Dependencies)
 └── README.md        (Project description)

Keep project organized → Judges like clean structure.
---

⚠️ IMPORTANT SECURITY WARNING

You shared:

MongoDB password

Connection strin

GitHub repo details


🚨 Never share:

Database passwords

API key's 

MongoDB URIs

GitHub tokens

Instead, use .env file:

MONGO_URI=your_connection_string

And add this to .gitignore:

.env

This keeps your database safe.


---

🧠 Golden Rule for Hackathon

Before coding:

git pull origin main

After coding:

git add .
git commit -m "clear message"
git push origin main

If confused:

git status


---

If you want, I can now give:

✅ Git branching notes
✅ Backend deployment steps
✅ MongoDB secure setup guide
✅ Complete hackathon workflow diagram

Tell me what you need next.
