# windows-terminal
Customising my Windows terminal with a Catppuccin Mocha theme, a JetBrains Mono Font, and Fastfetch.
--- 
## IMPORTANT!
This is adapted from the youtube tutorial provided by sleepycathey: https://www.youtube.com/watch?v=z3NpVq-y6jU
I am writing down my own step-by-step process and configurations for this.
--
# Steps
## JSON File
1. Go into terminal branch in aryali06/windows-terminal and find settings.json. Alternatively, use https://github.com/SleepyCatHey/Ultimate-Win11-Setup/blob/main/Terminal/settings.json for the original sleepycathey configuration which will use the JetBrains Mono Nerd Font.
2. Copy the code and open Windows Terminal.
3. In the dropdown section next to the new tab, click 'Settings' <img width="296" height="240" alt="image" src="https://github.com/user-attachments/assets/ec56c16b-7a32-476d-a566-553970ef5fd0" />
4. In the bottom bar, fine 'Open JSON file' and click it. Use Notepad or your preferred code editor.
5. Press Ctrl + A to select all code, delete it, and press Ctrl + V to paste in the code you copied. <img width="521" height="596" alt="image" src="https://github.com/user-attachments/assets/b9eab59c-5d27-4ddd-a167-a2fa849c799f" />
6. Press Ctrl + S to save changes and close the file.
7. When you open another tab, the theme will change to Catppuccin Mocha and the font is now your choice.

## Profile Creation
1. Check the location of your profile using $PROFILE in the terminal.
2. Make your way to that location. If the folder is empty, paste the code 'New-Item -Path $profile.CurrentUserAllHosts -Type File -Force' and press Enter. This will create the new profile.
3. You should see a PowerShell/WindowsPowerShell folder. Open it to find a 'profile.ps1' file. Close File Explorer upon confirmation. <img width="682" height="25" alt="image" src="https://github.com/user-attachments/assets/743e3949-b3de-46d8-8ceb-e4446b1b186e" />
4. Access the fastfetch repo here: https://github.com/fastfetch-cli/fastfetch
5. Copy the script 'winget install fastfetch' from the GitHub (or here) and paste it into terminal.
6. When it is installed, find the fastfetch branch in aryali06/windows-terminal, or https://github.com/SleepyCatHey/Ultimate-Win11-Setup/tree/main/Fastfetch for the sleepycathey config file and ascii art file. Download both files.
7. Open File Explorer and go to: This PC -> C: -> Users -> (your username) and create a new folder called '.config'. This is where you will store the downloaded config and ascii file.
8. Create a folder named 'fastfetch' and paste the two files in there.
9. Open the config file and change %USERPROFILE% to your username, save changes and close the editor.
10. Right-click the .config folder, choose 'Show More Options' and click Properties. Tick on the 'hidden' checkmark in attributes, click Apply, then click OK. <img width="353" height="450" alt="image" src="https://github.com/user-attachments/assets/edc694ab-1baa-4f60-9fad-d4c8018e7e33" />
11. Go back to your PowerShell 'profile.ps1' file and open it. Copy the code from the powershell branch in aryali06/windows-terminal or https://github.com/SleepyCatHey/Ultimate-Win11-Setup/blob/main/PowerShell/Microsoft.PowerShell_profile.ps1 and paste it in, replacing %USERPROFILE% with your username.
12. Ctrl + S to save changes and close the editor. Open a new tab in your terminal, and you are done! <img width="1990" height="1076" alt="Screenshot 2026-07-05 225902" src="https://github.com/user-attachments/assets/592f4806-40a5-4fc7-bd07-0891aab6f312" />
