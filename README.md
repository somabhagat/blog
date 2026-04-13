# 🚀 Antigravity Blog Project & Setup Guide

This repository contains my personal blog HTML files and Antigravity workspace settings. 

## 💻 How to Set This Up on a New PC
If you are reading this from a brand new computer, follow these steps to get back to work:

### 1. Install Git
- Download Git for Windows.
- **Important:** If using a secondary drive (like `Q:`), remember the path! (e.g., `Q:\Program Files\Git`).
- During installation, ensure "Add to PATH" is checked.

### 2. Configure Your Identity (The "Who Am I" Step)
Open **Git Bash** (search for it in the Start Menu) and type these two commands so Git knows who is saving the work:
- `git config --global user.email "bhagatsoma@gmail.com"`
- `git config --global user.name "somabhagat"`

### 3. Connect to GitHub (The "Handshake")
To allow the PC to upload to your private account without a password:
- Open Git Bash and run: `git config --global credential.helper manager`
- The first time you "Push," a window will pop up. Sign in via your browser.

### 4. Fix the Antigravity Source Control and Terminal
If the colorful terminal (Git Bash) doesn't show up inside the Antigravity editor:
1. Press `Ctrl + Shift + P` and search for **"Open User Settings (JSON)"**.
2. Add the path to the git executable: `"git.path": "Q:\\Program Files\\Git\\bin\\git.exe"` (This is the step that finally made the "Download Git" button disappear and showed your files in the Source Control (left panel))
3. In the **Workspace Settings** (this file: `blog.code-workspace`), ensure the terminal profile points to: `Q:\\Program Files\\Git\\bin\\bash.exe`.

### 🔧 The "Nuclear Option": Windows Environment Variables
If you have updated the JSON settings and Antigravity *still* doesn't see Git, you must tell Windows itself to broadcast the location of the Q: drive tools.

**Where to give this command:**
This isn't a terminal command; it's a Windows System setting.

1.  **Open Settings:** Press the `Windows Key`, type **"Edit the system environment variables"**, and hit Enter.
2.  **Access Variables:** Click the **Environment Variables** button at the bottom right.
3.  **Find 'Path':** In the bottom box labeled **System Variables**, scroll until you find **Path**, select it, and click **Edit**.
4.  **Add the Secret Paths:** Click **New** on the right side and paste these two paths (one at a time):
    * `Q:\Program Files\Git\bin`
    * `Q:\Program Files\Git\cmd`
5.  **Save & Reboot:** Click **OK** on all three windows. You **MUST restart Antigravity** (and possibly your PC) for this to take effect.

**Why this works:** By adding these to the "System Path," you are telling every app on your computer: "If you need a tool called 'git', you can find it in the Q: drive folder."

---

## 📝 Daily Workflow (How to Save)
Don't use the Windows Command Prompt. Use the **Terminal window at the bottom of Antigravity** (make sure it says `bash`).

### Step 1: See what you changed
Type this to see a list of modified files:
`git status`

### Step 2: "Pack the Lunchbox" (Stage changes)
You must tell Git which files are ready to be saved. To include EVERYTHING you changed:
`git add .`
*(The dot means "everything in this folder".)*

### Step 3: "Take the Photo" (Commit)
This saves a permanent snapshot to your computer's history with a note:
`git commit -m "Write a note here about what you did"`

### Step 4: "Upload to Cloud" (Push)
This sends your saved snapshots from your PC to your private GitHub repository:
`git push origin main`

---

## 📂 Project Structure
- `/blog`: Main folder containing all HTML posts.
- `blog.code-workspace`: The brain of the editor (contains drive paths).
- `.gitignore`: A list of junk files Git should ignore.