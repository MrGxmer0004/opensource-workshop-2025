# Module 2: The Workbench (VS Code & Editors)

![Workshop Status](https://img.shields.io/badge/Workshop-Live-green?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)
![PRs](https://img.shields.io/badge/PRs-Welcome-orange?style=for-the-badge)

## 1. Why Notepad Isn’t Enough
You cannot write production level code in Notepad or Google Docs. Code is not just text; it is logic that requires structure, syntax highlighting, and formatting standards.

For Open Source contribution, your editor is not just a typing tool; it is your command center. It needs to handle three things simultaneously:

* **Editing**: Writing the code.
* **Version Control**: Managing Git changes.
* **Execution**: Running the code (Terminal).

## 2. The Standard: Visual Studio Code (VS Code)
We are using VS Code. It is currently the industry standard for web and general purpose development. It is lightweight, open source, and runs everywhere.

### Why VS Code dominates Open Source:
* **Integrated Terminal**: You don't need to Alt Tab between your code and your command line. The terminal lives inside the editor. This is crucial for running Git commands alongside your code.
* **Git Integration (GUI)**: While you must learn CLI (Command Line Interface) commands, VS Code provides a visual representation of changes (diffs). You can see exactly what lines you changed before you commit.
* **Extensions**: Open source projects often require specific formatting (Prettier, ESLint). VS Code allows you to install these extensions so your code matches the project's standards automatically.

> **Crucial Note:** If your code format is wrong, your PR (Pull Request) will be rejected. You will be taught how to make a proper PR in this course later on.

## 3. The Alternatives (And why we aren't using them)
You will hear about other editors. Here is the honest breakdown of why they exist and why you shouldn't worry about them right now.

| Editor | The Verdict |
| :--- | :--- |
| **Sublime Text** | Incredibly fast, but requires manual setup. Good for quick edits, bad for beginners. |
| **IntelliJ / WebStorm** | Powerful Heavyweights. Full IDEs. Resource heavy and often cost money. Overkill for us. |
| **Vim / Neovim** | The Keyboard only editors. A nightmare for beginners. **Do not use today.** |
| **Atom** | Dead. Deprecated by GitHub. Do not use. |

## 4. Setup for the Workshop
To ensure you can follow the Open Source Workflow, we need to tweak VS Code immediately after installing it.

### Step A: Installation
* **Windows/Mac/Linux:** [Download from the Official Website](https://code.visualstudio.com/download)
* **Installation Note:** If asked during installation, check the box that says **Add to PATH**. This allows you to open VS Code from your terminal later.

### Step B: The Life Saver Settings
By default, VS Code makes you manually save files (`Ctrl+S`). Beginners often change code, forget to save, run the code, and wonder why nothing changed. Let's fix that.

1. Open VS Code.
2. Go to **File** > **Auto Save** (or search "Auto Save" in Settings).
3. Set it to `afterDelay` (1000ms).
   * *Why?* Now your code saves 1 second after you stop typing. You will never lose work again.

### Step C: Installing Essential Extensions
Extensions are what make VS Code powerful.
1. Click the **Extensions Icon** on the left sidebar (It looks like four squares with one floating away).
2. Search for and install these specific tools:

| Extension | Why we need it |
| :--- | :--- |
| **Prettier - Code formatter** | It forces your code to look professional. No more messy indentation. |
| **Git Graph** | Adds a button to visualize the "train tracks" of your Git history. |
| **Live Share(Optional)** | Allows you to code with a friend in real-time (like Google Docs for code). |

### Step D: The Terminal Check
We will be using the CLI (Command Line) heavily. VS Code has one built-in so you don't need to switch windows.
1. Press `` Ctrl + ` `` (The backtick key usually above Tab).
2. A panel should slide up from the bottom.
3. Type `echo "Hello World"` and press Enter.
4. If it prints "Hello World", you are ready.

### Step E: The Pro Move (The `code` command)
Developers don't open VS Code by clicking an icon. They open it from the folder they are working on.
1. Open your standard computer terminal (cmd or Terminal).
2. Type `code .` and press Enter.
3. **Did VS Code open?**
   * **Yes:** Great, your PATH is set up.
   * **No:** You likely missed the checkbox in Step A. Re install or ask a mentor for help.

That's a wrap for setting up the work bench VS Code. Now moving on to the soul of open source, [Module 3: Git Installation & Setup](../module-03-git-setup/01-installation.md).
