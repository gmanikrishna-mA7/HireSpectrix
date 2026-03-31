# HireSpectrix
Fake Job Detecting System.
Hola! Mi Yamo Mani Krishna, ¿está bien?.

# 💼 Fake Job Detection & Awareness System

The Fake Job Detection & Awareness System is a web-based application designed to help users identify suspicious job postings and avoid online job scams.

Many job seekers fall victim to fake job advertisements that promise high salaries, require registration fees, or use unprofessional communication methods. This project provides a simple and effective way to analyze job details and determine the risk level.

The system evaluates multiple factors such as salary, email domain, job description, and payment requirements to generate a risk score and classify the job as Safe, Medium Risk, or High Risk.

This project is built using HTML, CSS, and JavaScript, making it lightweight, fast, and easy to use.
🎯 A simple cybersecurity-focused mini project to spread awareness about job scams.

✅ File Structure (GitHub Section)
## 📁 Project Structure

fake-job-detector/

- │
- ├── index.html        # Home Page
- ├── analyze.html      # Job Analysis Form
- ├── result.html       # Result Display Page
- │__ support.html      # support page
- |__ contact.html      #contact Page
- |__ about.html        #About Page
- ├── style.css         # Styling (UI Design)
- ├── script.js         # Logic & Detection System
- │__ support.js        # Support system
- |__ contact.js        # Contact System
- └── images/           # (Optional) Icons / Assets

## ⚙️ How It Works

1. User opens the application and navigates to the Job Analysis page.

2. User enters job details such as:
   - Job Title
   - Company Name
   - Salary Offered
   - Contact Email
   - Job Description
   - Registration Fee (Yes/No)

3. When the user clicks "Analyze Job", the system processes the input using JavaScript logic.

4. The system checks for suspicious factors:
   - Unrealistically high salary
   - Use of free email domains (Gmail, Yahoo, etc.)
   - Requirement of registration/payment fee
   - Presence of suspicious keywords in job description

5. A risk score is calculated based on these conditions.

6. The result page displays:
   - Risk Level (Safe / Medium / High Risk)
   - Reasons for classification
   - Visual indicator (color or risk meter)

7. The user also gets awareness tips to avoid job scams.


✔ Analyze job postings for potential scams  
✔ Rule-based risk scoring system  
✔ Detection of suspicious keywords  
✔ Email domain validation  
✔ Registration fee warning system  
✔ Clean and responsive UI  
✔ Interactive design with animations  
✔ Awareness tips for users  


✅ Technologies Used
## 🛠️ Technologies Used

- HTML5
- CSS3
- JavaScript 

# ----------------------------------------------------------------------------------
# GIT-HUB
I want to share that how i created repositary.
# These is how to create a Repositary in Terminal
You can create a Git repository from the terminal in two main ways depending on what you want 👇
1. Create a LOCAL repository (basic way)
# go to your project folder
->cd "your-project-path"

# initialize git
->git init
👉 This creates a hidden .git folder → now your project is a Git repo
->git add .
->git commit -m "Initial commit"

2. Connect to GitHub (create remote repo)
-> In github Click on New Repositary
->copy repo URL
# In teriminal
->git remote add origin [https://github.com/your-username/repo-name.git] or [copy repo URL].git
->git branch -M main
->git push -u origin main.

# Now How to work with a branches like(dev,feature) and switching between them.

Core Idea
main → final / stable code (production)
dev → testing / combined development
feature → individual work (your duplicate/copy)
->You NEVER work directly on main.
Your “Duplicate Copy” = Branch

Instead of copying folders manually
Git gives you branches (lightweight copies)
->by these reason we create a Copys.
->Step 1: Start from main
git checkout main
git pull origin main
->Step 2: Create a duplicate branch (feature)
git checkout -b feature-login(This is your copy to work safely)
-> After doing your work or edits
->Step 3: Save your work
git add .
git commit -m "Added login feature"
->Step 4: Push your duplicate branch
git push -u origin feature-login
->Merge into dev branch..
git checkout dev
git merge feature-login(Merge your feature into dev)
git push origin dev(Push dev)
->Final: Move to main (after completion)
git checkout main(Switch to main)
git merge dev(Merge dev into main)
git push origin main(Push main)

# structure
main  ← stable
  ↑
dev   ← testing
  ↑
feature-login
feature-ui
feature-api
# some Rules to not get conflict
✔ Never work directly on main
✔ Always create a branch (feature)
✔ Merge → dev → then → main

# NOW how to delete branches after Merging
Once your feature is merged, you should clean it up
->Delete LOCAL branch
git branch -d feature-login(these is not a good approch beacuse it is force delete and deletes in your computer.)
->Delete REMOTE branch (GitHub)
git push origin --delete feature-login(Removes branch from GitHub)

# Now PULL REQUESTS
What is a Pull Request?
A Pull Request (PR) means:
“I finished my work → please review and merge into main/dev”.
🚀 Real Team Workflow
Step 1️⃣ Create feature branch
git checkout -b feature-login
Step 2️⃣ Work & commit
git add .
git commit -m "Added login feature"
Step 3️⃣ Push branch
git push origin feature-login
Step 4️⃣ Create Pull Request (on GitHub)

Go to your repo → you’ll see:

👉 “Compare & Pull Request” button

Click it

Step 5️⃣ PR Details
Base branch → dev or main
Compare branch → feature-login
Add title + description
Step 6️⃣ Review process

Team members:

Check your code 👀
Suggest changes ✏️
Approve ✅
Step 7️⃣ Merge PR

Click:
👉 Merge Pull Request

Step 8️⃣ Delete branch (recommended)

GitHub gives button:
👉 “Delete branch”

🧩 3. Types of PR merges
Type	Meaning
Merge commit	Keeps full history
Squash merge	Combines commits into one
Rebase merge	Clean linear history

👉 Most beginners use Merge commit

🔥 4. Why companies use PR

✔ Code review (avoid bugs)
✔ Team collaboration
✔ Clean history
✔ Track changes
✔ Prevent breaking main

🧠 5. Interview Explanation (IMPORTANT)

If interviewer asks:

👉 “What is Pull Request?”

You can say:

Pull Request is a feature in GitHub where developers submit their changes from a branch and request it to be reviewed and merged into another branch like main or dev. It helps in code review, collaboration, and maintaining code quality.

⚡ 6. Full Workflow Summary
# create branch
git checkout -b feature-login

# work
git add .
git commit -m "done"

# push
git push origin feature-login

# create PR on GitHub

# after merge
git checkout main
git pull origin main

# delete branch
git branch -d feature-login
git push origin --delete feature-login
🎯 Final Understanding
Branch = your safe workspace
PR = request to merge
Delete branch = cleanup

# 🔍 1. See commit message in terminal
✅ Command:
git log

👉 Output will look like:

commit 8a7f3c2...
Author: Your Name
Date: ...

    done

✔ That "done" is your commit message

⚡ Short version (clean view)
git log --oneline

👉 Example:

8a7f3c2 done
5b2a1d0 Updated README
🌐 2. See on GitHub

Go to your repository on GitHub

👉 Click:

"Commits" section

You’ll see:

done
Updated README
Added login feature
🧠 3. Where it appears in workflow

Every time you run:

git commit -m "done"

👉 Git creates a snapshot with label "done"

🎯 Best Practice

Instead of:

git commit -m "done"

Use meaningful messages:

git commit -m "Fixed login bug"
git commit -m "Updated UI design"

👉 Helps in:

Debugging 🔍
Team understanding 👥
Interviews 🎯
⚡ Bonus (see changes + message together)
git log -p

👉 Shows:

Commit message
Actual code changes
✅ Final Answer

✔ Use git log or git log --oneline
✔ Or check GitHub commits section
✔ "done" is stored as the commit label


# How I commit the changes 
🔍 Simple understanding
Git only tracks changes (differences), not entire files again and again.
🧠 What happens internally
When you do:
git add .
git commit -m "message"

👉 Git will:
Look at what files are modified / new / deleted
Store only those changes
Not duplicate unchanged content
📌 Example
First commit:
README.md → 100 lines
Second commit:
You change 2 lines

👉 Git stores:

Only those 2 changed lines, not entire 100 lines again
✅ So your statement is correct:

✔ Only changed files are added
✔ Only changes inside files are stored
✔ Unchanged files are ignored

⚡ One more clarity
Command	What happens
git add .	Stages all changed files
git add README.md	Stages only README
git commit	Saves staged changes only

2️⃣ Check what changed
git status
👉 You should see README.md in modified files

3️⃣ Add the README file
git add README.md
(Or use git add . to add everything)

4️⃣ Commit the changes
git commit -m "Updated README file".

5️⃣ Push to GitHub
git push origin main
✅ Done!

Your updated README will now appear on your GitHub repo..