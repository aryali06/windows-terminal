<div align="center">

# 🌺 windows-terminal 🌺

### *a cozy makeover for the windows terminal*

![Theme](https://img.shields.io/badge/theme-Catppuccin%20Mocha-f5c2e7?style=for-the-badge)
![Font](https://img.shields.io/badge/font-JetBrains%20Mono-cba6f7?style=for-the-badge)
![Tool](https://img.shields.io/badge/extra-Fastfetch-fab387?style=for-the-badge)

</div>

---

## About

This repo documents how I customised my Windows Terminal with a soft **Catppuccin Mocha** theme, the **JetBrains Mono** font, and a **Fastfetch** system-info splash 🖥️🎀

> Adapted from [sleepycathey's YouTube tutorial](https://www.youtube.com/watch?v=z3NpVq-y6jU) — this is my own step-by-step version with my personal configs and notes 📝

---

## Table of Contents

- [Part 1 — Theme & Font Setup](#-part-1--theme--font-setup)
- [Part 2 — PowerShell Profile & Fastfetch](#-part-2--powershell-profile--fastfetch)
- [Result](#-result)

---

## Part 1 — Theme & Font Setup

**Goal:** apply the catppuccin mocha theme + jetBrains mono font via `settings.json`.

| Step | What to do |
|:---:|---|
| 1 | Grab `settings.json` from the `terminal` branch of `aryali06/windows-terminal`, or use the original [SleepyCatHey config](https://github.com/SleepyCatHey/Ultimate-Win11-Setup/blob/main/Terminal/settings.json) (uses the Nerd Font version) |
| 2 | Copy the code, then open **Windows Terminal** |
| 3 | Click the dropdown ⌄ next to the new tab button → **Settings** |
| 4 | In the bottom-left corner, click **Open JSON file** (opens in Notepad or your editor of choice) |
| 5 | `Ctrl + A` to delete everything, then `Ctrl + V` to paste your copied config |
| 6 | `Ctrl + S` to save, then close the file |
| 7 | Open a new tab: your theme and font are now live |

<details>
<summary>📸 Reference screenshots</summary>
<br>

<img width="296" alt="Settings dropdown" src="https://github.com/user-attachments/assets/ec56c16b-7a32-476d-a566-553970ef5fd0" />
<img width="521" alt="Pasting JSON config" src="https://github.com/user-attachments/assets/b9eab59c-5d27-4ddd-a167-a2fa849c799f" />

</details>

---

## Part 2 — PowerShell Profile & Fastfetch

**Goal:** set up a powershell profile that runs **fastfetch** on every new tab 

| Step | What to do |
|:---:|---|
| 1 | Check your profile path by typing `$PROFILE` in the terminal |
| 2 | Navigate to that location. If it's empty, run:<br>`New-Item -Path $profile.CurrentUserAllHosts -Type File -Force` |
| 3 | You'll now see a `PowerShell` / `WindowsPowerShell` folder → open it to find `profile.ps1` |
| 4 | Head to the [fastfetch repo](https://github.com/fastfetch-cli/fastfetch) |
| 5 | Install it by running:<br>`winget install fastfetch` |
| 6 | Grab the config + ASCII art files from the `fastfetch` branch of `aryali06/windows-terminal`, or [SleepyCatHey's Fastfetch folder](https://github.com/SleepyCatHey/Ultimate-Win11-Setup/tree/main/Fastfetch) |
| 7 | In File Explorer: `This PC → C: → Users → (your username)` → create a new `.config` folder |
| 8 | Inside `.config`, create a `fastfetch` folder and drop both downloaded files in there |
| 9 | Open the config file, replace `%USERPROFILE%` with your actual username, save & close |
| 10 | Right-click `.config` → **Show more options** → **Properties** → tick ✅ **Hidden** → **Apply** → **OK** |
| 11 | Open `profile.ps1`, then paste in the code from the `powershell` branch of `aryali06/windows-terminal` (or [SleepyCatHey's profile script](https://github.com/SleepyCatHey/Ultimate-Win11-Setup/blob/main/PowerShell/Microsoft.PowerShell_profile.ps1)) — remember to swap `%USERPROFILE%` for your username |
| 12 | `Ctrl + S` to save, close the editor, then open a fresh tab — you're done! |

<details>
<summary>📸 Reference screenshots</summary>
<br>

<img width="682" alt="PowerShell profile folder" src="https://github.com/user-attachments/assets/743e3949-b3de-46d8-8ceb-e4446b1b186e" />
<img width="353" alt="Hidden folder attribute" src="https://github.com/user-attachments/assets/edc694ab-1baa-4f60-9fad-d4c8018e7e33" />

</details>

---

## Result

<div align="center">
<img width="1990" alt="Final terminal result" src="https://github.com/user-attachments/assets/acf0cd6e-cbae-4359-bd7c-cd7942ec5b44" />

**a soft, pretty, fully personalised terminal that you will actually want to use**
</div>

---

<div align="center">

*made with 🩷 by arya*

</div>
