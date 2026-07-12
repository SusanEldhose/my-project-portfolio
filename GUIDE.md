# Step-by-Step Guide: Setting Up Your GitHub Project Portfolio

This guide walks you through creating a GitHub repository from scratch, adding your first project (the Plant Phenomics mini-project), and adding future projects the same way.

---

## Part 1 — One-time setup

### Step 1: Create a GitHub account (skip if you already have one)

1. Go to [https://github.com](https://github.com)
2. Sign up with your email, choose a username, and verify your account.

### Step 2: Install Git on your computer

- **Windows:** download and install from [https://git-scm.com/download/win](https://git-scm.com/download/win)
- **Mac:** open Terminal and run `git --version` — if it's not installed, macOS will prompt you to install it (or use `brew install git`)
- **Linux:** `sudo apt install git` (Debian/Ubuntu) or your distro's package manager

Verify it worked:
```bash
git --version
```

### Step 3: Tell Git who you are (one-time, on this computer)

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```
Use the same email as your GitHub account.

---

## Part 2 — Create the repository

### Step 4: Create a new (empty) repository on GitHub

1. Log in to GitHub → click the **+** icon (top right) → **New repository**
2. Name it something like `my-project-portfolio`
3. Choose **Public** (so others can see it) or **Private**
4. **Do NOT** check "Add a README" — you already have one
5. Click **Create repository**
6. Copy the repository URL shown (looks like `https://github.com/your-username/my-project-portfolio.git`)

### Step 5: Download the files I've prepared

I've built the folder structure below for you (attached to this conversation):

```
portfolio-repo/
├── README.md
├── GUIDE.md
└── projects/
    └── plant-phenomics-trait-extraction/
        ├── README.md
        └── Mini_Project_Akanksha_Susan.pdf
```

Download it and unzip it on your computer wherever you'd like to keep your local copy (e.g. `Documents/my-project-portfolio`).

### Step 6: Turn the folder into a Git repository and push it

Open a terminal **inside** that folder, then run:

```bash
cd path/to/my-project-portfolio      # go into the unzipped folder

git init                             # start a new git repo here
git add .                            # stage all files
git commit -m "Initial commit: add plant phenomics mini-project"

git branch -M main                   # rename default branch to main
git remote add origin https://github.com/your-username/my-project-portfolio.git
git push -u origin main               # upload everything to GitHub
```

Replace `your-username/my-project-portfolio.git` with the URL you copied in Step 4.

If prompted for credentials, GitHub no longer accepts your password directly — use a **Personal Access Token** instead:
- GitHub → Settings → Developer settings → Personal access tokens → Generate new token → give it `repo` scope → use it in place of your password when Git asks.

### Step 7: Verify

Refresh your repository page on GitHub — you should see `README.md`, `GUIDE.md`, and the `projects/` folder with your presentation inside.

---

## Part 3 — Adding a new project in the future

Whenever you finish a new project, repeat this pattern:

### Step 1: Create a new folder

```bash
mkdir -p projects/name-of-new-project
```

### Step 2: Add your files

Put the project's files (code, slides, reports, images, etc.) inside that folder.

### Step 3: Add a `README.md` inside the new project folder

At minimum, include:
- **Title** and short description
- **Objective** — what problem it solves
- **Methodology / Approach** — how it works
- **Results** — what you found or built
- **Tools/Tech used**

### Step 4: Update the main `README.md`

Add a new row to the projects table pointing to the new project's README.

### Step 5: Commit and push

```bash
git add .
git commit -m "Add [project name]"
git push
```

That's it — your portfolio grows one project at a time, always visible at:
`https://github.com/your-username/my-project-portfolio`

---

## Tips

- **Large files:** GitHub blocks files over 100 MB by default. Your current `.pdf` (~1.5 MB) is well under that limit, but keep this in mind for future projects with large videos, datasets, or embedded media — use [Git LFS](https://git-lfs.com/) if you ever hit the cap.
- **.gitignore:** for future code projects, add a `.gitignore` file to avoid committing things like `node_modules/`, `.venv/`, or `__pycache__/`.
- **Keep READMEs consistent:** using the same structure (Objective → Methodology → Results) for every project makes your portfolio easy to skim.
