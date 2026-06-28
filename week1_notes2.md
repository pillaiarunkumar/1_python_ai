# 📋 Python AI — Class 1 

## Summary
Mayank Aggarwal opened the first session, covering class logistics, learning expectations, and foundational toolchain setup. He introduced UV as the preferred Python package and project manager, explained why a Linux-compatible terminal matters, and live-demonstrated creating and activating virtual environments. The session established the base stack (Python 3.10+, VS Code, UV, terminal) that the entire course builds on.

## Key Concepts
- **UV** — Rust-based Python package and project manager, ~200x faster than pip; install packages with `uv pip install` or `uv add`
- **Virtual Environment (venv)** — Isolated Python environment per project with its own packages and Python version; created via `uv venv --python 3.12`
- **Package Manager** — Tool (pip, UV, Conda, Poetry) for fetching and installing third-party Python libraries
- **Git Bash** — Linux-compatible terminal for Windows; lets Windows users run the same Unix-style commands as cloud servers
- **Excalidraw + Craft Link** — Visual whiteboard + shared resource page updated each class with all commands, prompts, links, and notes

## Topics Discussed

### Course Structure and Expectations
- Sessions start at 8:00 AM IST; no waiting beyond 8:05 from the next class onward
- Pomodoro format: 15–20 min teaching blocks + 5 min Q&A; one break ~9:30 AM; dedicated doubt session after 11 AM
- Zoom chat is one-way (student → instructor only, not peer-to-peer by design)
- All resources (code, commands, prompts, notes) shared via a single Craft link — bookmark and refresh it each class
- Recordings shared after every session; course avoids unnecessary student spending (uses free tiers, Grok, Open Router)
- Do not use office laptops — corporate restrictions block scripts and cause errors that can't be debugged

### 4-Class Course Roadmap
- Class 1: Python AI fundamentals (today — environment, packages, virtual envs)
- Class 2: Pydantic — structured output, essential for agentic systems
- Class 3: GenAI vs AI vs Agents — concepts taught without any framework dependency
- Class 4: Build a minimal manual agent in pure Python to solidify fundamentals
- Post-month: LangChain, LangGraph, and other frameworks introduced after strong foundations are in place

### Toolchain Setup
- **Python 3.10+**: download from python.org; 3.13.x recommended; both `python` and `python3` commands should resolve to 3.10+
- **VS Code**: free, industry-standard IDE; also provides a built-in Linux-compatible terminal
- **UV**: Mac/Linux install: `curl -LsSf https://astral.sh/uv/install.sh | sh`; Windows: PowerShell command from UV docs; also `pip install uv`
- **Terminal**: Mac/Linux have Unix terminals by default; Windows users must install Git Bash or Windows Terminal — PowerShell/CMD are insufficient for real development
- Cloud/production servers almost always run Linux — learning Linux-style commands now pays off immediately when deploying

### Python Versions and Virtual Environments
- `python` and `python3` can point to different installations; both must be 3.10+ — the version itself doesn't matter as long as it meets that floor
- Virtual environments isolate each project's packages so versions don't conflict across projects
- Create: `uv venv --python 3.12` | Activate (Mac/Linux): `source .venv/bin/activate` | Windows: `.venv\Scripts\activate`
- Packages installed inside a venv are unavailable outside it — demonstrated live: `import requests` failed outside the venv, worked inside
- Each venv can have a different Python version; UV handles downloading the right version automatically

### Package Management Philosophy
- UV preferred over pip/conda/poetry for speed and modern AI-era workflows
- Python is "vanilla ice cream"; packages are toppings — third-party code written by others that extends Python
- Use `uv pip install <pkg>` or `uv add <pkg>` inside an active virtual environment
- Never memorize code — use AI (ChatGPT/Claude) for command lookup; focus on understanding the logic
- Reading documentation is the single skill that accelerates careers — it's the only source of truth, including for AI output

## Action Items
1. **All students**: Install Python 3.10+ from python.org before the next class
2. **All students**: Install VS Code from code.visualstudio.com
3. **All students**: Install UV — Mac/Linux: `curl -LsSf https://astral.sh/uv/install.sh | sh`; Windows: PowerShell command from UV docs
4. **Windows students**: Install Git Bash from git-scm.com to get a Linux-compatible terminal
5. **All students**: Bookmark the shared Craft link and refresh it at the start of every class
6. **All students**: Switch to a personal laptop — do not use office laptops for this course
7. **All students**: Practice creating and activating a virtual environment before the next class
Read less
